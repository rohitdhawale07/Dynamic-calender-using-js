# Dynamic-calender-using-js

## Hosted Link :- https://rohitdhawale07.github.io/Dynamic-calender-using-js/

This is project of creating a Dyanmic calender which highlights todays date or date we enter.
We can simply select a year ranging from 1900 to 2099 and any month from dropdowns as shown.
Firstly we created html code for calender using select and option tag for years ,months and days of month whether it is 30 or 31.
In the bottom we used form tag and inside it created input tag and enter button.
## HTML code
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calender</title>
    <link rel="stylesheet" href="./style.css">
    <script defer src="./index.js"></script>
</head>
<body>
    <div class="main">
        <div class="container">
            <section class="month-year">
                <select class="select-month">
                    <option disabled selected value="">Select Month</option>
                    <option value="0">January</option>
                    <option value="1">February</option>
                    <option value="2">March</option>
                    <option value="3">April</option>
                    <option value="4">May</option>
                    <option value="5">June</option>
                    <option value="6">July</option>
                    <option value="7">August</option>
                    <option value="8">September</option>
                    <option value="9">October</option>
                    <option value="10">November</option>
                    <option value="11">December</option>
                </select>
            <select class="select-year">
             <option selected disabled>Select Year</option>
             <option>1900</option><option>1901</option><option>1902</option><option>1903</option><option>1904</option><option>1905</option><option>1906</option><option>1907</option><option>1908</option><option>1909</option><option>1910</option><option>1911</option><option>1912</option><option>1913</option><option>1914</option><option>1915</option><option>1916</option><option>1917</option><option>1918</option><option>1919</option><option>1920</option><option>1921</option><option>1922</option><option>1923</option><option>1924</option><option>1925</option><option>1926</option><option>1927</option><option>1928</option><option>1929</option><option>1930</option><option>1931</option><option>1932</option><option>1933</option><option>1934</option><option>1935</option><option>1936</option><option>1937</option><option>1938</option><option>1939</option><option>1940</option><option>1941</option><option>1942</option><option>1943</option><option>1944</option><option>1945</option><option>1946</option><option>1947</option><option>1948</option><option>1949</option><option>1950</option><option>1951</option><option>1952</option><option>1953</option><option>1954</option><option>1955</option><option>1956</option><option>1957</option><option>1958</option><option>1959</option><option>1960</option><option>1961</option><option>1962</option><option>1963</option><option>1964</option><option>1965</option><option>1966</option><option>1967</option><option>1968</option><option>1969</option><option>1970</option><option>1971</option><option>1972</option><option>1973</option><option>1974</option><option>1975</option><option>1976</option><option>1977</option><option>1978</option><option>1979</option><option>1980</option><option>1981</option><option>1982</option><option>1983</option><option>1984</option><option>1985</option><option>1986</option><option>1987</option><option>1988</option><option>1989</option><option>1990</option><option>1991</option><option>1992</option><option>1993</option><option>1994</option><option>1995</option><option>1996</option><option>1997</option><option>1998</option><option>1999</option><option>2000</option><option>2001</option><option>2002</option><option>2003</option><option>2004</option><option>2005</option><option>2006</option><option>2007</option><option>2008</option><option>2009</option><option>2010</option><option>2011</option><option>2012</option><option>2013</option><option>2014</option><option>2015</option><option>2016</option><option>2017</option><option>2018</option><option>2019</option><option>2020</option><option>2021</option><option>2022</option><option>2023</option><option>2024</option><option>2025</option><option>2026</option><option>2027</option><option>2028</option><option>2029</option><option>2030</option><option>2031</option><option>2032</option><option>2033</option><option>2034</option><option>2035</option><option>2036</option><option>2037</option><option>2038</option><option>2039</option><option>2040</option><option>2041</option><option>2042</option><option>2043</option><option>2044</option><option>2045</option><option>2046</option><option>2047</option><option>2048</option><option>2049</option><option>2050</option><option>2051</option><option>2052</option><option>2053</option><option>2054</option><option>2055</option><option>2056</option><option>2057</option><option>2058</option><option>2059</option><option>2060</option><option>2061</option><option>2062</option><option>2063</option><option>2064</option><option>2065</option><option>2066</option><option>2067</option><option>2068</option><option>2069</option><option>2070</option><option>2071</option><option>2072</option><option>2073</option><option>2074</option><option>2075</option><option>2076</option><option>2077</option><option>2078</option><option>2079</option><option>2080</option><option>2081</option><option>2082</option><option>2083</option><option>2084</option><option>2085</option><option>2086</option><option>2087</option><option>2088</option><option>2089</option><option>2090</option><option>2091</option><option>2092</option><option>2093</option><option>2094</option><option>2095</option><option>2096</option><option>2097</option><option>2098</option><option>2099</option></select>                
            </section>

         <section class="calender">
            <ul class="week">
                <li>Sun</li>
                <li>Mon</li>
                <li>Tues</li>
                <li>Wed</li>
                <li>Thu</li>
                <li>Fri</li>
                <li>Sat</li>
            </ul>
            <ul class="day">
                <li class="days"></li>
                <li class="days"></li>
                <li class="days"></li>
                <li class="days"></li>
                <li class="days"></li>
                <li class="days">1</li>
                <li class="days">2</li>
                <li class="days">3</li>
                <li class="days">4</li>
                <li class="days">5</li>
                <li class="days">6</li>
                <li class="days">7</li>
                <li class="days">8</li>
                <li class="days">9</li>
                <li class="days">10</li>
                <li class="days">11</li>
                <li class="days">12</li>
                <li class="days">13</li>
                <li class="days">14</li>
                <li class="days">15</li>
                <li class="days">16</li>
                <li class="days">17</li>
                <li class="days">18</li>
                <li class="days">19</li>
                <li class="days">20</li>
                <li class="days">21</li>
                <li class="days">22</li>
                <li class="days">23</li>
                <li class="days">24</li>
                <li class="days">25</li>
                <li class="days">26</li>
                <li class="days">27</li>
                <li class="days">28</li>
                <li class="days">29</li>
                <li class="days active">30</li>
                <li class="days"></li>
                <li class="days"></li>
            </ul>
         </section>

         <form class="date" onsubmit="ValidateDate(event)">
            <input type="number" placeholder="Enter Date" min="1" max="31" required="" class="EnterDate">
            <input type="submit" class="submit" value="Enter">
           </form>

        </div>
    </div>


</body>
</html>

```
For CSS styling we used flex properties, hovering proerties,margin, padding, borders, align items etc as below.
## CSS Code
```
*{
    margin: 0;
    padding: 0;
    font-family: cursive;
}
.main{
    width: 100%;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: url(https://www.topcu.org/wp-content/uploads/Annual-Meeting-Calendar-background-1.jpg);
    background-size: cover;
}
.container{
    width: 60%;
    height: 70%;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    box-shadow: rgba(252, 250, 250, 0.35) 0px 5px 15px;    
    border-radius: 10px;
    background-color: rgba(0,0,0,0.7);
}
.month-year{
    width: 96%;
    height: 15%;
    display: flex;
    align-items: center;
}
select {
    font-size: larger;
    padding: 1%;
    margin-right: 2%;
}
.calender {
    width: 96%;
    height: 60%;
}
.calender ul {
    display: flex;
    list-style: none;
    flex-wrap: wrap;
}
.calender ul li {
    width: calc(100%/7);
    text-align: center;
    padding-top: 1.5%;
    color: white;
    font-weight: 550;
}
.calender ul li:hover{
    background-color: rgb(224, 253, 218);
    color: black;
}
.active {
    background-color: green;
    border-radius: 5px;
}
.week{
    font-size: larger;
    height: 15%;
}
.week>li {
    background-color: rgba(246, 247, 245, 0.5);
}
.day {
    height: 85%;
}
.date {
    width: 96%;
    height: 15%;
}
form {
    display: flex;
    align-items: center;
}
.EnterDate {
    font-size: larger;
    padding: 1%;
    margin-right: 2%;
    width: 20%;
}
.submit {
    font-size: larger;
    padding: 1%;
    background-color: royalblue;
    color: white;
    border: none;
    border-radius: 5px;
}
.submit:hover{
    background-color: white;
    color: black;
    scale: 1.03;
    cursor: pointer;
}
```
For Javascript Part we used differnt events and event listener.
firstly we get all the ids by using document.getElementById() method and stored in variables.
firstly we created function named dateOfFirstDay() which will return the first day of each month. 
we get today day, month and year by using getDate() method.
we applied simple logic here that next years first day will be exceeding by one day with respect to previuos year.
fillDates() this function will return the number of days present in a perticular month.
The month numbering 0,2,4,6,7,9,11 will present 31 days.
The month numbering except above months will consists 30 days.
And for feb month first we will check if year is leap (that is if year is divisible by 4) then there will be 29 days in month otherwise there will be 28 days in a feb month.
For highlighting the seletced date or todays date we used highlightColor() function.
For taking inputs of selected year and selected month we used takeinputs() function which will return the selected year and month.
We add event listner to the enter button of type click event .
## JAVASCRIPT Code
```
const current = new Date();
const date = current.getDate();
const month = current.getMonth();
const year = current.getFullYear();
const daysList = document.querySelectorAll(".days");

function dateOfFirstDay(month, year) {
  daysList.forEach((ele) => {
    ele.innerHTML = "";
  });
  const total = new Date(`${month + 1} 1, ${year} 23:15:30`);
  const day = total.getDay();
  fillDates(day, month, year); 
}

function fillDates(day, month, year) {
   
  if (
    month === 0 ||
    month == 2 ||
    month == 4 ||
    month == 6 ||
    month == 7 ||
    month == 9 ||
    month == 11
  ) {
    let count = 1;
    for (var i = day; i < 31 + day; i++) {
      if (i >= day) {
        daysList[i].innerText = count;
        count++;
      }
    }
  } else if (month == 1) {
    let count = 1;
    if (year % 4 === 0) {
      for (var i = day; i < 29 + day; i++) {
        if (i >= day) {
          daysList[i].innerText = count;
          count++;
        }
      }
    } else {
      for (var i = day; i < 28 + day; i++) {
        if (i >= day) {
          daysList[i].innerText = count;
          count++;
        }
      }
    }
  } else {
    let count = 1;
    for (var i = day; i < 30 + day; i++) {
      if (i >= day) {
        daysList[i].innerText = count;
        count++;
      }
    }
  }
  highlightColor(date);
}
dateOfFirstDay(month, year);

function highlightColor(date) {
    daysList.forEach(ele=>ele.classList.remove("active"))
  daysList.forEach((ele) => {
    if (ele.innerHTML == date) {
      ele.classList.add("active");
    }
  });
}


function fillingYears() {
  const yearList = document.querySelector(".select-year");
  for (let i = 1900; i < 2100; i++) {
    const option=document.createElement("option")
    option.innerText=i;
    yearList.appendChild(option)
    
  }
}
fillingYears();

function takeinputs(){
    const month=document.querySelector(".select-month").value;
    const year=document.querySelector(".select-year").value;
    if(month==="Select Month"){
        const newmonth=new Date().getMonth();
        dateOfFirstDay(+newmonth,+year)
    }
    else if(year==="Select Year"){
      const newyear=new Date().getFullYear();
      dateOfFirstDay(+month,+newyear);
    }
    else{
        dateOfFirstDay(+month,+year)
    }
}
document.querySelector(".select-month").addEventListener("change",takeinputs)
document.querySelector(".select-year").addEventListener("change",takeinputs)

function ValidateDate(e) {
    e.preventDefault();
    const date=document.querySelector(".EnterDate")
    highlightColor(date.value)
    date.value=""
}
```




