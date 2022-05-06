![img](images/cover-logo.png)

## Support

**Flutter debugPrint** is an extension created for **Visual Studio Code**.

## Flutter debugPrint

Easily insert and remove `debugPrint('variable: $variable');` statement.

[![Version](https://vsmarketplacebadge.apphb.com/version/ricardo-emerson.flutter-print.svg)](https://marketplace.visualstudio.com/items?itemName=flutter-debugprint.flutter-debugprint)
[![Install](https://vsmarketplacebadge.apphb.com/installs/flutter-debugprint.flutter-debugprint.svg)](https://marketplace.visualstudio.com/items?itemName=flutter-debugprint.flutter-debugprint)
[![Downloads](https://vsmarketplacebadge.apphb.com/downloads/flutter-debugprint.flutter-debugprint.svg)](https://marketplace.visualstudio.com/items?itemName=flutter-debugprint.flutter-debugprint)
[![Ratings](https://vsmarketplacebadge.apphb.com/rating-star/flutter-debugprint.flutter-debugprint.svg)](https://marketplace.visualstudio.com/items?itemName=flutter-debugprint.flutter-debugprint&ssr=false#review-details)

# Usage Examples

> This extension overrides the shortcut for **Select all occurrences of current selection** - `Ctrl+Shift+L` on Windows and Linux and `Cmd+Shift+L` on macOS, however you can still use `Ctrl+F2` to execute same command.

## Print for variables

Select the variable that you want uses print statement and press `Ctrl+Shift+L` on Windows, Linux or macOS.

![Usage](images/print-variable.gif)

## Print for object properties

Select the object properties that you want uses print statement and press `Win+Shift+L` on Windows and Linux or `Cmd+Shift+L` on macOS.

![Usage](images/print-object.gif)

## Remove all print statements

To remove all print statements and press `Win+Shift+D` on Windows and Linux or `Cmd+Shift+D` on macOS.

![Usage](images/delete-log.gif)

# With Custom Log Class

Create a custom log class.

```dart
import 'dart:developer' as developer;

class Log {
  Log._();

  static void print(String value) {
    developer.log(value, name: 'LOG');
  }

  static Object? inspect(Object? object) {
    developer.inspect(object);
  }
}
```

## Log.print() for variables

Select the variable that you want uses a custom Log.print statement and press `Win+Ctrl+L` on Windows and Linux or `Cmd+Ctrl+L` on macOS.

![Usage](images/log-print-variable.gif)

## Log.print() for object properties

Select the object properties that you want uses a custom Log.print statement and press `Win+Alt+L` on Windows and Linux or `Cmd+Alt+L` on macOS.

![Usage](images/print-object.gif)

## Log.inspect() for variables

Select the variable that you want uses a custom Log.inspect statement and press `Win+Ctrl+L` on Windows and Linux or `Cmd+Ctrl+L` on macOS.

![Usage](images/log-inspect.gif)

**That's all, Enjoy!**

original source: <https://marketplace.visualstudio.com/items?itemName=ricardo-emerson.flutter-print>
