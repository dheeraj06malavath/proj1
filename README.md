1. Setup repo locally

git clone <repo_url>

2. Verify remote connections

git remote -v

3. Check status (staged/unstaged/untracked)

git status

4. Create + switch to new branch

git checkout -b feature/<name>

5. List branches (local + remote + current)

git branch -a

6. Add specific file + commit

git add <file>
git commit -m "message"

7. Add missed file to last commit (no message change)

git add <file>
git commit --amend --no-edit

8. Fetch remote changes without modifying working dir

git fetch

9. Pull latest changes into current branch

git pull origin main

10. Rebase feature branch onto updated main

git rebase main

11. Abort rebase

git rebase --abort

12. Undo a faulty commit (keep history)

git revert <commit_id>

13. Undo last commit but keep changes staged

git reset --soft HEAD~1

14. Remove file from version control but keep locally

git rm --cached <file>

15. Stash uncommitted changes

git stash

16. View stashes + apply

git stash list
git stash apply

17. Compare branches for specific file

git diff main feature/<branch> -- <file>

18. One-line commit graph

git log --oneline --graph --all

19. Merge feature branch into main

git checkout main
git merge feature/<branch>

20. Push and verify sync

git push origin main
git status
🔹 EXTRA GIT (from other sets edge cases)

Initialize repo + first commit

git init
git add .
git commit -m "initial commit"

Show differences

git diff

Unstage file

git reset <file>

Switch branch

git checkout <branch>

Recover lost commit

git reflog
git checkout <commit_id>

Force push after rebase

git push origin <branch> --force
🔹 DOCKER CLI (from all sets combined)





1. Clone repo + enter dir

git clone <repo_url>
cd <repo>
ls

2. Build Docker image

docker build -t <image_name> .

3. Run container (background + port mapping)

docker run -d -p 8080:8080 --name <container_name> <image_name>

4. Show running containers

docker ps

5. Show all containers

docker ps -a

6. Enter running container

docker exec -it <container_name> /bin/bash

7. Stop container

docker stop <container_name>

8. Start container

docker start <container_name>

9. Commit container to image

docker commit <container_id> <username>/<image>:v1

10. Login to Docker Hub

docker login

11. Push image to Docker Hub

docker push <username>/<image>:v1

12. Logout

docker logout
🔹 EXTRA DOCKER (other sets)

Tag image

docker tag <image> <username>/<repo>:tag

View images

docker images

View logs

docker logs <container>

🔹 GIT CLI COMMANDS

1. Setup repo locally

git clone <repo_url>

2. Verify remote connections

git remote -v

3. Check status (staged/unstaged/untracked)

git status

4. Create + switch to new branch

git checkout -b feature/<name>

5. List branches (local + remote + current)

git branch -a

6. Add specific file + commit

git add <file>
git commit -m "message"

7. Add missed file to last commit (no message change)

git add <file>
git commit --amend --no-edit

8. Fetch remote changes without modifying working dir

git fetch

9. Pull latest changes into current branch

git pull origin main

10. Rebase feature branch onto updated main

git rebase main

11. Abort rebase

git rebase --abort

12. Undo a faulty commit (keep history)

git revert <commit_id>

13. Undo last commit but keep changes staged

git reset --soft HEAD~1

14. Remove file from version control but keep locally

git rm --cached <file>

15. Stash uncommitted changes

git stash

16. View stashes + apply

git stash list
git stash apply

17. Compare branches for specific file

git diff main feature/<branch> -- <file>

18. One-line commit graph

git log --oneline --graph --all

19. Merge feature branch into main

git checkout main
git merge feature/<branch>

20. Push and verify sync

git push origin main
git status
🔹 EXTRA GIT

Initialize repo + first commit

git init
git add .
git commit -m "initial commit"

Show differences

git diff

Unstage file

git reset <file>

Switch branch

git checkout <branch>

Recover lost commit

git reflog
git checkout <commit_id>

Force push after rebase

git push origin <branch> --force
🔹 DOCKER CLI COMMANDS

1. Clone repo + enter dir

git clone <repo_url>
cd <repo>
ls

2. Build Docker image

docker build -t <image_name> .

3. Run container (background + port mapping)

docker run -d -p 8080:8080 --name <container_name> <image_name>

4. Show running containers

docker ps

5. Show all containers

docker ps -a

6. Enter running container

docker exec -it <container_name> /bin/bash

7. Stop container

docker stop <container_name>

8. Start container

docker start <container_name>

9. Commit container to image

docker commit <container_id> <username>/<image>:v1

10. Login to Docker Hub

docker login

11. Push image to Docker Hub

docker push <username>/<image>:v1

12. Logout

docker logout
🔹 EXTRA DOCKER

Tag image

docker tag <image> <username>/<repo>:tag

View images

docker images

View logs

docker logs <container>
