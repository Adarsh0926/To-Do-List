# To-Do-List
To Do List using JS
<!DOCTYPE html>
<html>
    <head>
        <title>ToDO</title>
    </head>

    <body>

        <input type="text" id="new_list_item">
        <button onclick="addItem()">Add item</button>

        <!-- 1. Create a List-->
        <!-- 2. Give 2 default list items-->
        <script type="text/javascript">
            var listItems = ['Buy Groceries', 'Make Breakfast'];
        </script>
        <script type="text/javascript">
            function addItem()
            {
                var tempItem = document.getElementById("new_list_item").value;
                listItems.push(listItems);
                displayList(tempItem);
                document.getElementById("new_list_item").value = '';
            }
        </script>


        <!-- 3. Display the list-->
        <div id="Display">
            <h3>Your ToDo : </h3>
            <ul>
                <script type="text/javascript">
                    listItems.forEach(displayList);

                    function displayList(item)
                    {
                        document.getElementById("Display").innerHTML += "<li>"+item+"</li>"
                    }
                </script>
            </ul>
        </div>
        <!-- 4. Add items to the list-->
    </body>


</html>
