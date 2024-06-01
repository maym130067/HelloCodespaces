# HelloCodespaces

This is just a test repository. Pay no mind and have a good day.

1. Create repository

2. Create a Codespace VM

3. Modify the README file

4. Work in Terminal:
    ls                          || lists files in current directory and finds filename for compilation for running from terminal
    ls -al                      || gives more info on contents of directory
                                . is current directory
                                .. is the parent directory
                                .git directory that has info about the current git repository
    more fileName               || shows contents of file, such as for the README.md
    git status                  || shows status (ex. modified/unmodified) of files in directory
    git add fileName            || stages file for push
    git add .                   || adds current file that you are working on
    git commit -m "yourMessage" || commits all staged files and adds change message
    git push                    || pushes changes to remote (account level) repository
    clear                       || clears terminal to give you a clean terminal
    java --version              || tells you the current version of java in the codespaces VM
    javac --version             || tells you the current version of the java compiler
    javac fileName.java         || compiles .java file and creates a class file (compiled version [bytecode] for jvm to run on any OS) -->
    java fileNameWithoutDotJava || runs the program (bytecode class file) (same as pressing the run button in upper right)
    After command syntax (ex. javac ), type letters of file until distinct --> press tab || autocompletes filename
    rm fileName.class || removes class file

5. Stop codespace when not working on it to conserve available minutes left
    https://github.com/codespaces has your active codespaces listed and you can stop them from here
    yourHoursAvailable(120 for free version) / numberOfCoresOnCodespaceCPU (basic is 2 cores) = yourHoursLeftForMonth;

6. file explorer --> right click This PC --> choose properties --> choose advanced system settings --> 
click Environment Variables --> click Path in bottom window --> Click edit --> put directory of wanted 
version of java above (or in front if single line) others to make current default java version

7. Do not save class file since it is only for running a single instance of the program so -->
create new file, file name as .gitignore --> # is the comment symbol --> at top of .gitignore type: 
# Compiled Class File
--> line 2 type: *.class  tells github to ignore any(wildcard [asterisk]) class with the suffix .class. 
Make sure to add, commit, and push the .gitignore file and check repository (no .class and shows .gitignore). 
git status command should no longer show class file and class file should be greyed out as well in codespace

8. Debug summary: https://www.udemy.com/course/learn-github-codespaces-for-java-development/learn/lecture/35686970#overview