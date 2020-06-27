# password [-chf]

Randomly generate / locate a unique password in your command line interface of choice. All passwords are stored on a text file with readability permissions removed

Syntax: password [-chfar] [LABEL]

c     Create unique password with associated label

h     Display help page

f     Find previously generated password by searching all labels

a     Read all labels and their respective passwords

r     Remove label and their respective passwords 

R     Force remove file that saves all passwords

Examples:
$ password -c YouTube
	YouTube Password: m49958Xv$
  
$ password -c Facebook
	Facebook Password: D31145HE$
  
$ password -c YouTube
	Error: duplicate label called 'YouTube' found

$ password -f Facebook
	Facebook Password: D31145HE$
  
$ password -a
	YouTube    m49958Xv$
	Facebook   D31145HE$
  
$ password -r YouTube
	Successfully removed password for 'YouTube'

$ password -a
	Facebook   D31145HE$

$ password -R
	Force remove passwords.txt file [y/n]: y
  
  Succesfully removed all passwords
