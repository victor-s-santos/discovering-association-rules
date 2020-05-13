<table>
   <tr>
      <p align="center">
        <a href="#about">About</a> •
        <a href="#how_to_run">How to run</a> •
        <a href="#introductory">Introductory</a> •           
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
    * git clone https://github.com/victor-s-santos/Python-SQL.git

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
>This path where I do demonstrate of apyori python use from a very simple false market shopping note. I also demonstrate how the params are be calculated by the algorithm. 

<tr>
    <p align="center">
        <a href="https://github.com/victor-s-santos/discovering-association-rules/tree/master/introductory/" target="_blank">Simple Case</a>           
    </p>
</tr>