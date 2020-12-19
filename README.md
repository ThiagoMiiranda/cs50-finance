<h1 align="center">CS50x-Finance</h1>
<p align="center">
	A web application to simulate buying and selling on the stock exchange. Built in Python 3 using Flask framework, SQL database and IEX API. This is a solution to the Harvard University's CS50x problem set - web track.
</p>
<div>
    <p align="center">
        <a href="https://www.python.org/" target="_blank">
            <img src="https://img.shields.io/static/v1?label=Python&message=v.3.9.1&color=blue&style=%3CSTYLE%3E&logo=python" alt="python">
        </a>
        <a href="https://flask.palletsprojects.com/en/1.1.x/" target="_blank">
            <img src="https://img.shields.io/static/v1?label=Flask&message=v.1.1.2&color=blue&style=%3CSTYLE%3E&logo=flask" alt="flask">
        </a>
    </p>
</div>
<p align="center">
    <a href="#status-and-access">Status and Access</a> •
    <a href="#specification">Specification</a> •
	<a href="#pre-requirements">Pre Requirements</a> •
	<a href="#how-to-run">How to run</a>
</p>
<h2>Status and Access</h2>
<div align="center">
    <p>✅ Concluded</p>
    <p>
        <a href="https://cs50webtrack-finance.herokuapp.com/login" target="_blank">
            <img src="https://img.shields.io/static/v1?label=Heroku&message=CS50x-Finance&color=green&style=%3CSTYLE%3E&logo=heroku" alt="cs50x-finance">
        </a>
    </p>
    <img src="https://raw.githubusercontent.com/ThiagoMiiranda/cs50-finance/main/static/cs50-finance.jpg" alt="cs50x-finance">
</div>
<h2>Specification</h2>
<p>
    This is a solution to the 2nd exercise from the web track/problem set proposed by Harvard University's CS50x, Introduction to Computer Science. The website contains a simple interface made with bootstrap and uses IEX's free API to query for shares prices in real time.
</p>
<p>
    The problem ask you to implement the following features:
    <ul>
        <li>Create a database with one or more tables to store enough information without being redundant.</li>
        <li>Create HTML files that extends from an existing layout with the appropriate content.</li>
        <li>Allow a user to <strong>register</strong> for an account.</li>
            <ul>
                <li>Hash the user password before storing it.</li>
            </ul>
        <li>Allow the user to <strong>consult</strong> a stock's current price.</li>
        <li>Allow the user to <strong>buy</strong> and <strong>sell</strong> stocks with cash in account.</li>
        <li>Create an <strong>index</strong> page where the user can see a table containing all the stocks it currently have.</li>
            <ul>
                <li>Have to show which stocks, the number of shares, the current price of each stock, the total value of each holding and also display the user's current cash along with a grand total (total holdings + cash).</li>
            </ul>
        <li>Create an <strong>history</strong> page where the user can see a table containing all the transactions the user has ever made.</li>
            <ul>
                <li>Have to show which stocks, the number of shares, the price of each stock the moment it was bought, the total value of each holding and also display the date and time of each.</li>
            </ul>
        <li>A personal touch</li>
    </ul>
</p>
<h3>My personal touch</h3> <p>
    I added a new collumn on the index page that has two buttons (buy/sell) that only appears when the user hovers over it. It's a quality of life improvement where the user wouldn't have to type in again the name of each stock they already own.
</p>
<h2>Pre Requirements</h2>
<p>
    Before begin, you will need to install in your PC <a href="https://www.python.org/" target="_blank">Python</a> and <a href="https://flask.palletsprojects.com/en/1.1.x/" target="_blank">Flask</a>.
</p>
<h2>How to run</h2>
First, you need to download the repository in a .zip file or clone it using git:

```
git clone https://github.com/ThiagoMiiranda/cs50-finance.git
```
Open your terminal and `cd` into the directory

```
cd \cs50-finance\venv\Scripts
```
Run `activate.bat`
You should see a "(venv)" before directory path
Execute `cd..` 2 times to go back to \cs50-finance
Now set initial variables
(if using linux instead of set type `export`)

```
set FLASK_APP=application.py
set API_KEY=pk_ac8702e833ce4a13af5c3064903130de
```
Lastly, run the application
`flask run`
