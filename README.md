# html-
learning record about html
2023/8/14 5:44 pm 
heres my conclusion about how to use html well:) 
One thing is important-CSS cascading whatwhatwhat;
so the basic form starts with <style> and normally the 
crucial title are without"." but your diy should have one.
 <style>
    body {
      font-family: Arial, sans-serif;
      color:black
    }
    .container {
      width: 80%;
      margin: 0 auto;
      border: 1px;
      background-color: burlywood;
to make a table its much more difficult with CSS;
.outerbox{
border: 2px solid black;

padding: 10px;
display: inline-block;
background-color: cornflowerblue;
text-align: center;
            }  to make a outerbox 
     then use like <div>to set separated blocks.
     use <tr> for each row and <td> for each element.
<!DOCTYPE html>
<html>
    <HEAD>
        <title>tour web design</title>
    </HEAD>
    <style>
body{
    background-image: url('1.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-attachment: fixed;
    color: rebeccapurple;
    text-align:center;
    font-size: 24px;
    
}
    </style>
    <body>
        <div><h1>hello!</h1><br>
        Welcome to tourweb!where you can meet different senic spots!
    </body>
</div>
<div>
   <p> plz fill these Information so that we can serve you better :)</p>
   
   <form>
   Your name: <input type="text" name="name"><br>
    area: <input type="text" name="area"><br>
    contact: <input type="text"name="area"><br>
    Your Gender:<br>
    Male<input type="radio" name="Gender" value="Male"><br>
    Female<input type="radio"name="Gender"><br>
 </form>
 <form method="post">
    where you want to go?<select name="places">
        <option value ="1">ASIA</option>
        <option value ="2">AMERICA</option>
        <option value ="3">AFRICA</option>
        <option value ="4">EUROPE</option>
        <option value ="5">OCEANIA</option>
    </select>
    <br>
    Thank you for your cooperation!Click "Submit" for your results!<br>
    <input type="Submit" value="Submit!"></input>
 </form>
</div>
</html>

 <!DOCTYPE html>
<html>
<head>
    <style>
        table {
            border-collapse: collapse;
            width: 100%;
            table-layout: fixed;
        }
        th, td {
            border: 1px solid brown;
            padding: 8px;
            text-align: center;
            width: 25%;
        }
        th {
            background-color: brown;
            color: white;
        }
    </style>
</head>
<body>
    <table>
        <tr>
            <th>X</th>
            <th>X^2</th>
            <th>1/x</th>
            <th>x^1/2</th>
        </tr>
        <!-- 使用 JavaScript 生成表格行 -->
        <script>
            var table = document.querySelector('table'); // 获取表格元素
            for (var i = 1; i <= 5; i++) {
                var row = document.createElement('tr'); // 创建<tr>元素
                var cell1 = document.createElement('td');
                var cell2 = document.createElement('td');
                var cell3 = document.createElement('td');
                var cell4 = document.createElement('td');
                
                cell1.textContent = i;
                cell2.textContent = i * i;
                cell3.textContent = (1 / i).toFixed(2);
                cell4.textContent = Math.sqrt(i).toFixed(2);
                
                row.appendChild(cell1);
                row.appendChild(cell2);
                row.appendChild(cell3);
                row.appendChild(cell4);
                
                table.appendChild(row); // 将<tr>添加到表格中
            }
        </script>
    </table>
</body>
</html>
