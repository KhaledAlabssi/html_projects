# Moon-trip Ticket

This HTML project designed for my Frontend course participants. The goal of this project is to let participants practice the real use/needs of HTML forms and inputs.

## Requirments:

- HTML (form and table)

## Build/Practice:

Build this project by checking out how it looks [here](https://html-cv.khaled.page), or by going through the steps below.

## Steps/Walkthrough:

#### Level 1

1. Create new folder and name it "form-data".
2. Navigate to "form-data" folder you just created using your editor, and create index.html file.
3. Initiate/declare the html file by typing "html:5" or "!" and select html:5.
4. Change the title (in head element) from Document to your "Moon Ticket Application".
5. Inside the body element, create `"h1"` element with "Free Ticket to the Moon" as a content.
6. Create `"h2"` element with "Apply now!!!" as a contnet.
7. Create `"form"` element. No need for action or methods attributes for this exercise.
8. Create `"input"` element for the "name" with proper type attribute, and id attribute with "name" as it's a value.
9. Create `"input"` element for the "email" with proper type attribute, and id attribute with "email" as it's value.
10. Create `"input"` element for the "password" with proper type attribute, and id attribute with "password" as it's value.
11. Create `"input"` element for the "number" of people will join the trip, with proper type attribute, and id attribute with "people" as it's value.
12. Create `"select"` element for the "reason of the trip" with some randome `"option"` element. add id attribute to `"select"` element with value of "reason".
13. Create `"input"` element for the "allergy question" with RADIO type attribute, and name attribute with "allergy" as it's value.
14. Create `"textarea"` element for the "Anything we should know?" with proper type attribute, and name attribute with "desc" as it's value.
15. Create `"input"` element for the "date" with proper type attribute, and id attribute with "date" as it's value.
16. Create `"input"` element for the "time" with proper type attribute, and id attribute with "time" as it's value.
17. Create `"input"` element for the "submit" with proper type attribute, add id and value attributes with "submit" as a value.
18. Create `"table"` element with id attribute of "table". Add to your table 8 `"th"` with proper values that matches the questions above.
19. Go up to `"head"` section, and paste the following code:
```
    <style type="text/css">
        table {
        display: none;
        }
        th, tr, td {
        border-bottom: 3px solid gray;
        }
    </style>
```
NOTE: please know that this code will be explained in future sessions :) 

20. Go back to the bottom of `"body"` section and paste the following code:
```
    <script type="text/javascript">
        document.getElementById("submit").onclick = function (e) {
        e.preventDefault()
        var table = document.getElementById("table")
        table.style.display = "block"

        var row = table.insertRow(-1)
        var name = row.insertCell(0)
        var email = row.insertCell(1)
        var people = row.insertCell(2)
        var reason = row.insertCell(3)
        var allergy = row.insertCell(4)
        var extra = row.insertCell(5)
        var time = row.insertCell(6)
        var date = row.insertCell(7)

        name.innerHTML = document.getElementById("name").value
        document.getElementById("name").value = "";
        email.innerHTML = document.getElementById("email").value
        document.getElementById("email").value = "";
        document.getElementById("password").value = "";

        people.innerHTML = document.getElementById("people").value
        document.getElementById("people").value = "";

        reason.innerHTML = document.getElementById("reason").value
        document.getElementById("reason").value = "";

        allergy.innerHTML = document.querySelector(
            'input[name="allergy"]:checked'
        ).value
        document.querySelector('input[name="allergy"]:checked').value = ""

        extra.innerHTML = document.getElementById("desc").value
        document.getElementById("desc").value = "";

        date.innerHTML = document.getElementById("date").value
        document.getElementById("date").value = "";

        time.innerHTML = document.getElementById("time").value
        document.getElementById("time").value = "";


        return false
        }
    </script>
```
NOTE: Please know that this code wi


## Before:
![Screenshot 2022-09-17 192820](https://user-images.githubusercontent.com/26570366/190869347-35b1f3bc-f0b4-4ace-9cd2-c11a8b286291.png)

## After:
![Screenshot 2022-09-17 193017](https://user-images.githubusercontent.com/26570366/190869363-5cfce7aa-d74f-4f72-9273-62ad4f480764.png)