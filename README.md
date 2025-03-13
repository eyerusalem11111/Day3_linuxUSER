# Day3_linuxUSER
user name=eyerusalem
Hostname=kali
Current Directory=Path/pwd/ the working directory at moment/
Previlage = $-(user),#-(root/ i can act like ruller of kali linux)
Home diectory is denoted by ''~" named telda/tilda
~ = /home/eyerusalem
local directoy/where my current directory/="-"
all directory is denoted by=""
Directory=folder
options -> are additional commands and added as --option arguments
arguments-> things that are input to have output eg.  maths/command/ --add/oprion/ 1 1/arguments/
**command
-> are words that can do one task 
ls -> list elements  of current directory
ls [option] [File] 
tree->structuraly lists elements of directory

ls -l =>add more details of elements
perm.txt=>permission
ls -a=> all hidden files are displayed
ls Desktop=>lists elements in Desktop
ls -R=> recursively lists elements
ls -Rla=>recursively detailed hidden information list
**Change directory/cd/
cd[existing directory] =>change and enter to indicated directory
cd /=> for root directory
cd =>for home directory or telda , same as cd ~
cd .. =>for 1 previous back

cd ../..=> for 2 previous back
~/gtst=> u ware in telda and now u are in gtst and can get back to telda as cd .. or cd

=>folder creation in  folder is hard for cd so one method is to cd " home gtst"


/root=> home  directory for all powerful users
/etc=> contain linux configuration files(control when and how programs start up)
/home=> the users home directory.
/mnt=> where other filesystems are attached or mounted to the filesystem.
/media=>where CDS and USB devices are usually attached  or mounted to the filesystem.
/bin=>where application binaries( the equivalent of executable in microsoft windows) resides.
/lib=> where shared liabraries are found
/=>root
cd .. .. =>to root
double dash (--) for like help
single dash (-)for single words like l,h,a
(--help,-h,-?)=>for help
eg.
nmap -help=>descriptions of nmap
man=>for lists of descriptions like module
eg. man aircrack-ng ->lists information about aircrack
to quit use (q)
**Finding Stuff
locate + to be found =>gives every detail  a lot of information of fully one day updated once not for less than 24 hours.
which=>only returns the binary in the path variable.
pwd=>print working directory,the output starts from / sign and it indicates root.
all folders start with /.
/ called root  directory.
 echo=>is command  for displaying  what is written after it as an  argument.
** output redirecting refers to putting  once output as input to the other.

in echo command we can redirect (writing in to a file) to using > sign
eg. echo "hello" > file.txt
put  and save hello in file.txt 
to check what file is contained in a echo we can use /cat/ command.
if i say cat echo
to add/redirect /save/ message to  existing file using echo we use (>>) 
cat,head,less,tail=> are used to show contents in a file.
*cat
=  cat test.txt=> displayes all content,starting from index 0
*less
=less test.txt==> displayes in a text editor which i am out using (q)

=tail
=  tail  text.txt==>display 10 lines from bottom to top starting from index  1.
=head
==> head test.txt ==>displayes 10 lines starting from 1 top to bottom

*
touch===>create text file of many number
like touch file file file
the file is empty inside.
eg. touch alazar bamlak
mkdir ==> make directory
eg. mkdir file file file

mkdir -p ==>creat folder inside a folder
eg. mkldir -p (new created folder->)desu/new created folder/(->)bro
folder is created with out space.
mkdir folder1 folder2 ===>creates two  folders
clear==>delete from the screan==(ctrl+l)
rm ==>remove file
eg. rm abrham alazar 
to delete directory that have file we use -r= delete recursively
                                 -i= forprompt(time  for desion)yes -> delete no--> not deleted
                                 -f=delete bu force that is not deleted
                                -rf=every thing is deleted weather it  it say i am undeleted.



cp==>copy
eg.cp  oldfile newfile/(newinside folder)
eg cp echo.txt menta=>copy to menta
cp echo.txt menta/abrham=>copy to abrham
mv===>move and save
mv oldfile newfile
to copy file on home diectory we use cp abrham/menta/echo.txt ~/menta\ wndi/
	cp -r=> copy the directory with all  its files.
	cp "cyber sec note.pdf" ../../tmp==>  copy the text to tmp in root
	now we are in tmp to  go to download and and copy we use ~/Download/
grep=>global search for regular expression ,displayes the line.

eg.grep "my" test.txt
	
grep -i ==>make the  search case insensitive.
grep  -c==>count number of line that the word is found.
grep -l * ==>displayes the directory  that  the word is found on.
grep -r===>searches a word in a folder in all files recursivelyg
grep -v==>display lines that are exclusive of the word being searched
grep -n==>display the number line with the word line
like 1: my my
grep -o==>display only the word searched.
grep -a==>search text in zip file.
grep -ran===>recursively search in all ziped files and display it with line number.
**wc/word count/
==> specifically tell the line (-l),word(-w),byte(-c)
of given  the file.


**Multiple command execution in one line.
And(&&)
works if two commands are out of error. and display the second line  of point
or(||)
command will be executed, if it have error or not.it is neccessaryto have the first command be error free
pipeing(|)
the first line output is the second line input.


sed/stream editor
 - process large file filter, word replacement, delete specific line, manipulation for penetration test
 - eg.  syntax->sed 'command' file
 - replace : sed 's/old/new/'
 - if the repkaced lineis written more than one use
 sed 's/old/new/g'
  - delete: sed '/word/d'  file
  awk 
  - aho,weinberger,kernghan
  - is is sed on structure files
- syntax: awk 'pattern { action}' file.txt
- awk '{print $1,$3}' file.txt / prints column1and 3
- awk '/condition/ {print $0}' file.txt
- awk by default determines colomns by space and the space is called the Delimiter
- to make it detect other colomns we use -F  ","
- conventions in awk - $0=entire linev of text
                    -$1,$2= represent each colomn(field) in a line
                    -NR: line(record ) number
                    -NF:number  of field in the current record,display the last colomn file.
u can use it with file or pipied.
- Awk'options' file.txt
- cat 'file.txt'|awk'options





