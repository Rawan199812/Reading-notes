## Permissions

**Permission checks are always run at the very start of the view, before any other code is allowed to proceed. Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.**


***How permissions are determined?***

**Before running the main body of the view each permission in the list is checked. If any permission check fails an exceptions.PermissionDenied or exceptions.NotAuthenticated exception will be raised, and the main body of the view will not run.**

**Setting the permission policy**
- The default permission policy may be set globally, using the DEFAULT_PERMISSION_CLASSES setting. 

REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.IsAuthenticated',
    ]
}

## Generic views

**One of the key benefits of class-based views is the way they allow you to compose bits of reusable behavior. REST framework takes advantage of this by providing a number of pre-built views that provide for commonly used patterns.**

## GenericAPIView

**This class extends REST framework's APIView class, adding commonly required behavior for standard list and detail views.**

- Each of the concrete generic views provided is built by combining GenericAPIView, with one or more mixin classes.

**Django REST framework is a powerful and flexible toolkit that makes it easy to build Web APIs. It provides class based generic API views and serializers. We've taken all the attributes and methods that every view/serializer defines or inherits, and flattened all that information onto one comprehensive page per class.**