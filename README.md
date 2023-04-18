# Notion Formulas
I am getting fond of notion and decided to create a repo where I can store the formulas I have created for my own workspace.

---
## Showing age of something
```javascript
if (
  dateBetween(now(), prop("Created at"), "hours") == 0,
    concat(format(dateBetween(now(), prop("Created at"), "minutes")), " minutes"), 
    if (
      dateBetween(now(), prop("Created at"), "hours") > 24,
        concat(format(dateBetween(now(), prop("Created at"), "days")), " days"),
        concat(format(dateBetween(now(), prop("Created at"), "hours")), " hours")
    )
)
```
### Result
<img width="1311" alt="image" src="https://user-images.githubusercontent.com/30486759/232695150-2e079bf2-0f49-4ebd-93b8-53ef77ec897c.png">
