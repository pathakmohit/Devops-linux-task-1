# Devops-linux-task-1  

#Task 1

- Create users and groups:
    o	Create users alice, bob, and carol.
    o	Create a group called devteam.
     o	Add bob and carol to devteam.
  
- Setup Project Directory:
    o	Create the /project directory.
    o	Assign ownership of /project to alice and group ownership to devteam.
    o	Set directory permissions so that alice and group members can read, write, and execute inside /project, but others have no access.
  
- Create files with specific permissions:
    o	As alice, create a project plan file project_plan.txt that only she can modify, but everyone can read.
    o	Create a source code directory /project/src owned by bob with group devteam, allowing bob and group members to add or modify files but deny others.
    o	Inside /project/src, create a script file build.sh, make it executable, but only bob can execute it; others can read it but cannot execute.
  
- Set default permissions for new files in /project/src: o	Configure the /project/src directory so that new files created by users inherit the group devteam.
    o	Ensure new files have permissions so that the owner can read/write and group can only read.
  
- User access tests: o	As carol, try to edit project_plan.txt (should fail).
     o	As bob, execute build.sh (should succeed).
     o	As carol, try to execute build.sh (should fail).
     o	As alice, view contents of /project/src and list file permissions.
