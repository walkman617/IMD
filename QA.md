## 1. What's the differece between '@+id/' and 'android:id'?

- The at-symbol (@) at the beginning of the string indicates that the XML parser should parse and expand the rest of the ID string and identify it as an ID resource. 
- The plus-symbol (+) means that this is a new resource name that must be created and added to our resources (in the R.java file). 
- There are a number of other ID resources that are offered by the Android framework. When referencing an Android resource ID, you do not need the plus-symbol, but must add the android package namespace, like so:
<strong>android:id="@android:id/empty"</strong>

## 2. Is RTC same as UTC or local time?

- RTC = Real Time Clock
- UTC = Universal Time Coordinated

They're not really the same thing. UTC basically means the same thing as the GMT time zone, or the Greenwich Mean Time. It's considered the "center" of all the time zones, and all *nix-based systems set & work with time based on this value by default.

The RTC is the device in your computer that keeps track of time even when the computer is turned off & unplugged. That's the reason for the CMOS battery in your system - - to keep the clock running, and to save certain BIOs settings.

The easiest way to set your RTC is to make sure that your Linux time zone & clock are properly set to your local time. Unless you've mucked around with hidden settings, that should automatically set your RTC to the correct UTC time. For example, my time zone is UTC-5. So if I set my clock in Linux for 8:00 AM, my BIOs clock is set to 1:00 PM automatically.