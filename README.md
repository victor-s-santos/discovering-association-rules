<table>
   <tr>
      <p align="center">
        <a href="#about">About</a> •
        <a href="#how_to_run">How to run</a> •
        <a href="#introductory">Introductory</a> •
        <a href="#real_case">01 - Real Case</a> •
        <a href="#pizzeria">02 - Pizzeria</a> •
        <a href="#entrance_exam">03 - Entrance Exam</a> •           
      </p>
   </tr>
</table>

# About
> This is repository where I am studying mainly about the apyori python algorithm. In this repository I am also looking for to explore the library Pandas instead of doing everything in SQL queries. 


# How_to_run
> To run this repository, follow the steps:
1. Create a virtualenv (this isn't necessary, but I belive this is a good practic):
    * python3 -m venv .venv `to create a virtualenv`
    * source .venv/bin/activate `to use this virtualenv`
    
2. Clone this repository:
    * git clone https://github.com/victor-s-santos/discovering-association-rules.git

3. Install the dependencies:
   * pip install ipython[notebook] `to install jupyter notebook`
   * python -m pip install python-dotenv `to install dotenv`
   * python -m pip install pymysql `to install this pure-Python MySQL client library`

   3.1 Graph dependencies:
      * python -m pip install matplotlib
      * python -m pip install seaborn
   
   *__obs:__ `python -m pip install is necessary to install the packages in the current jupyter notebook kernel. But you can also install from the browser:`
   >
    import sys

    !{sys.executable} -m pip install numpy

4. Run a python notebook:
    * ipython notebook
    
5. To see a Database manager:
    * Install Adminer: `sudo docker pull adminer`
    * Run Adminer
    sudo docker run \
        --name adminer \
        -p 8080:8080 \
        -d \
        adminer
    * Now you can create and populate your table from adminer  accessing: http://localhost:8080/
    * __obs:__`I am not giving the values to insert in the database, but I am giving the database schema.`


# Introductory
>This path where I do the demonstrate of apyori python use from a very simple false market shopping note. I also demonstrate how the params are be calculated by the algorithm. 

<tr>
    <p align="center">
        <a href="https://github.com/victor-s-santos/discovering-association-rules/tree/master/introductory/" target="_blank">Simple Case</a>           
    </p>
</tr>

# Real_Case
>Using a real simple note, I am going to implement the apyori and study about the returned result. Using this relation we can get good insights about the products and reach ideas to apply for increase the business. 

<tr>
    <p align="center">
        <a href="https://github.com/victor-s-santos/discovering-association-rules/tree/master/01-real%20case" target="_blank">Real purchase notes</a>           
    </p>
</tr>

# Pizzeria
>Using a real database from a pizzeria. In this section we can see the customer behavior, like what day most orders are done, what are the most comum included items for each order, etc. Using this knowledge the owner can be choose a better way to attract more clients or even a way to optimize their sales.  

<tr>
    <p align="center">
        <a href="https://github.com/victor-s-santos/discovering-association-rules/tree/master/02-pizzeria" target="_blank">Pizzeria</a>           
    </p>
</tr>

# Entrance_Exam
>Using the real database from answered questions about economic situation for each student whose did this entrance exam. The discovered rules in this section could be used to understand the public education situation. In comercial case, this rules could be used to offer better paymant conditions, to choose better places to execute the exam for instance.      

<tr>
    <p align="center">
        <a href="https://github.com/victor-s-santos/discovering-association-rules/tree/master/03-entrance_exam" target="_blank">Entrance Exam</a>           
    </p>
</tr>

# Apriori Params
* __Params__:

| __Suport__          | __Confidence__   | __Lift__            | __Length__         |
|-----------------|:-------------|:---------------:|---------------:|
| Support represent the frequency that respective item occours in the transaction| Confidence represents how reliable this result is  | Lift demonstrates how relevant the respective rule is      | Number of rules that are going to be returned|
| Should be provided by the user                | Should be provided by the user          | Should be provided by the user      | Should be provided by the user            |