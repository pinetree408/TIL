# @NonNull

The @NonNull annotation can be used to indicate that a given parameter can not be null.

If a local variable is known to be null (for example because some earlier code checked whether it was null),
and you pass that as a parameter to a method where that parameter is marked as @NonNull,
the IDE will warn you that you have a potential crash.
