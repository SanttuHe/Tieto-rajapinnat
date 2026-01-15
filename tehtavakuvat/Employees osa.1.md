A.  Employees-tietokannan osastojen nimet

&nbsp;	**SELECT Dept\_name**

      **->FROM departments;**



b) Mitä nimikkeitä tietokannassa title on

&nbsp;	**SELECT DISTINCT title**

      **->FROM titles;**



c) Pienin ja suurin palkka



&nbsp;	**SELECT** 

  	**MIN(salary) AS min\_salary,**

  	**MAX(salary) AS max\_salary**

	**FROM salaries;**

&nbsp;	



d) Keskimääräinen palkka



&nbsp;	**SELECT AVG(salary)**

      **->FROM salaries;**



e) Työntekijät, joiden sukunimi Facello



	**SELECT\***

      **->FROM employees**

      **->WHERE last\_name = 'Facello';**



f) Kuinka moni syntynyt 1950-luvulla



&nbsp;	**SELECT COUNT(\*) AS born\_in\_1950s**

       **-> FROM employees**

       **-> WHERE birth\_date BETWEEN '1950-01-01' AND '1959-12-31';**



g) Montako naista ja miestä on employees taulukossa



&nbsp;	**SELECT GENDER, COUNT(\*) AS count**

      **-> FROM employees**

      **->GROUP BY gender;**

