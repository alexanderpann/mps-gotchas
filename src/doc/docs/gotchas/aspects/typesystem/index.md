!!! warning  "Typesystem rules are not executing."

    Turn off the [power save mode](https://www.jetbrains.com/help/mps/status-bar.html?q=Power%20save%20mode). Also make sure that the languages that contains the rules is used. Make sure that under Tool->
    Model Checker the typesystem checks are enabled. Some rules are only checked when "Check model" is invoked. In this case the
    option "do not apply on the fly" is set to true in a checking rule.

!!! question  "Are comparison rules often used?"

    No, they are rarely used (not many results across various code bases).