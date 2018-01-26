# Log Analysis Project

## Submission for Full-Stack Web Developer Nanodegree
This project queries news database, organizes and prints the query results accordingly.

## Requirements:

- Virtualbox
    You can download virtualbox from [here](https://www.virtualbox.org/wiki/Downloads).
- Vagrant
    You can download vagrant from [here](https://www.vagrantup.com/downloads.html).
- Python
    You can download python [here](https://www.python.org/downloads/).

## Usage

1. Clone this project on github

    $ git clone https://github.com/sk15973/Log-Analysis-Project.git

2. Change directory to the project folder

3. run `vagrant up` from command line

4. Download the sql file from [here](https://d17h27t6h515a5.cloudfront.net/topher/2016/August/57b5f748_newsdata/newsdata.zip), extract the file and move it to the project folder.

5. after vagrant set up is complete run `vagrant ssh` and `cd /vagrant folder`.
    **Database setup**
    * Run the following commands once during the first time execution of the project.
    * `sudo su - postgres`
    * `psql`
    * `CREATE DATABASE news;`
    * `CREATE USER vagrant;`
    * `GRANT ALL PRIVILEGES ON DATABASE news to vagrant;`
    * `psql -d news -f newsdata.sql`

6. run `python LogAnalysis.py` to the get the results.

## SQL file
The SQL file was provided by udacity as part of the project course material.
Download the SQL file from [news data](https://d17h27t6h515a5.cloudfront.net/topher/2016/August/57b5f748_newsdata/newsdata.zip).

## Acknowledgments:
- Providing course and mentorship - [Udacity](https://in.udacity.com/).
- Documentations and code samples - [Python](http://www.python.org/).
