# **Gmail Emails Analyzer**

The project has two parts as described belows:

## **Part 1:** 

## Objective:

The aim of this project is to extract all the emails from your inbox using the GYB command line tool. It also uses regular expressions to extract particular data from the emails.

## Requirement

### Downloading all emails from your Gmail account

For this part, you need to install the GYB command line tool on your system.

To install the GYB command line tool simply clone the repository by using the command on the console-

```bash
git clone https://github.com/jay0lee/got-your-back.git
```

After cloning the repository you can follow the following steps to get your email data

1. `cd got-your-back`
2. Type `touch nobrowser.txt`
3. Run the command `python3 gyb.py --email youremail@gmail.com --action backup`
4. It will ask you for authentication of your email account. Copy the url into the web browser and authenticate the gmail account. A verification code shall be displayed. Copy that.
5. Paste the verification code on the console.

The emails shall be backed up in the folder `'got-your-back/GYB-GMail-Backup-youremail@gmail.com'`


## Insturctions

1. Install the **GYB command** line tool and Use the command line to download all the emails as described in the above section.
2. The emails get downloaded to a folder called `got-your-back/GYB-GMail-Backup-youremail@gmail.com`
3. Write a function which takes in the following parameters :
    1. Path of the folder where your emails are stored. 1, The field corresponding to which values need to be found, eg. to, from, body.
    2. The pattern to match, ie the regex pattern for an email.

Your function should find all the values which match the pattern provided to the function. For eg. calling the function -

```python
your_function(path='path_where_emails_are_backedup', field='to', pattern='regexpattern')
```

Should return all the email ids in the “to” field. We’ll be passing appropriate regex pattern for matching emails.

---

## **Part 2:** 

## Objective:

The objective of this project is to analyze the email data you collected in the previous project. This uses Python Numerical computation & analytics libraries e.g. Numpy, Scipy and Pandas to analyze the emails data for given objectives

## Insturctions

From the data you collected and the concepts you learned in the class (Numpy and dataframes in Pandas) do the following analysis on the data :

1. Find the top 5 times of the week when you receive the most number of emails. Hint. Categorise the data on the basis of time into slots and find the slot with the most number of emails.
2. Who has sent you the maximum number of emails?
3. To whom have you sent the maximum number of emails?
4. On the basis of above two analysis decide who is your closest buddy. You are free to derive your own formula for choosing your closest buddy. One of the criteria can be the person whom you converse frequently.


### Installing

This project requires installation of latest Anaconda distribution.

## Running the tests

Please refer to individual Jupyter notebook for inline instructions.

## Built With

* [Python 3.6](https://www.python.org/downloads/release/python-364/) - Programming Language used
* [CloudxLab](https://cloudxlab.com/lab//) - An integrated development environment on the cloud

## Authors

* **Noor Khemji** 

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* [People @cloudxlab](https://cloudxlab.com)
![Cloudxlab](https://cloudxlab.com/static/cxl/images/logo.png "CloudxLab")
