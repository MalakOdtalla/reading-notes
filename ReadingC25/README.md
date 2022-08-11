## DRF Permissions

In DRF, permissions, along with authentication and throttling, are used to grant or deny access for different classes of users to different parts of an API.

The simplest style of permission would be to allow access to any authenticated user, and deny access to any unauthenticated user.

### Permission classes
Permissions in DRF are defined as a list of permission classes. You can either create your own or use one of the seven built-in classes. All permission classes, either custom or built-in, extend from the BasePermission class.

BasePermission has two methods, has_permission and has_object_permission, that both return True.

- has_permission:  is used to decide whether a request and a user are allowed to access a specific view.

- has_object_permission:  is used to decide whether a specific user is allowed to interact with a specific object

<b> Built-in DRF Permission Classes</b>

- AllowAny

The AllowAny permission class will allow unrestricted access, regardless of if the request was authenticated or unauthenticated.


- IsAuthenticated

The IsAuthenticated permission class will deny permission to any unauthenticated user, and allow permission otherwise.
This permission is suitable if you want your API to only be accessible to registered users.


- IsAdminUser

The IsAdminUser permission class will deny permission to any user, unless user.is_staff is True in which case permission will be allowed.
This permission is suitable if you want your API to only be accessible to a subset of trusted administrators.

- IsAuthenticatedOrReadOnly

The IsAuthenticatedOrReadOnly will allow authenticated users to perform any request. Requests for unauthorised users will only be permitted if the request method is one of the "safe" methods; GET, HEAD or OPTIONS.
This permission is suitable if you want to your API to allow read permissions to anonymous users, and only allow write permissions to authenticated users.


To know more about permissions, see this [site](https://www.django-rest-framework.org/api-guide/permissions/#how-permissions-are-determined)