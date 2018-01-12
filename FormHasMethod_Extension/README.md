Extension to Global::formHasMethod() class that supports form methods added via extensions.

For methods with optional parameters it throws AmbiguousMatchException exception that is handled inside of Global_Extension class. However, we cannot catch it a transaction, so either don't use it the trassaction or handle AmbiguousMatchException exception outside of the trasaction. 
