mkdocs serve > mkdocs.log 2>&1 &
cat mkdocs.log

install mkdocs 
pip install mkdocs
pip install mkdocs-include-markdown-plugin


run for mkdocs
open environment 
source venv/bin/activate
1) mkdocs serve Protocol to protect connection

2) mkdocs serve --dirty

copy past 
cp /home/work/Pictures/Screenshots/tui-asset-data.png /home/work/code/jans/docs/assets

Copy from local and past in lxc 
-> lxc file push /home/ifour/Downloads/agama-pw.gama jans-host/tmp/

==================================================
docs-remove-newline-issues-and-trailing-spaces

for the roule apply 

install in the vs code
npm install -g markdownlint-cli@0.34.0

file name :
.markdownlint.json

{
  "default": false,
  "MD009": {
    "br_spaces": 0,
    "list_item_empty_lines": true
  },
  "MD047": true
}

run for all md file 
npx markdownlint "**/*.md" --fix


====================================================
Safe way to run git pull --rebase when you have local changes

git restore --staged . 
git stash 
git pull --rebase 
git stash pop

✅ 1. git restore --staged .

Unstages all files.

Anything you added with git add . is removed from the staging area.

Your changes stay in your working directory (not lost).

📌 Purpose: Make the index clean so the next stash works correctly.

✅ 2. git stash

Temporarily saves all your uncommitted changes (both staged and unstaged) and gives you a clean working directory.

Your files are saved in a hidden “stash”.

Your working directory becomes clean (no local edits).

📌 Purpose: Allow git pull --rebase to run without conflicts caused by your local changes.

✅ 3. git pull --rebase

Updates your branch by applying new remote commits, then adding your future commits on top (but for now you have no local commits because everything was stashed).

📌 Purpose: Get the latest code from the remote repository cleanly.

✅ 4. git stash pop

Restores your saved changes back into your working directory and removes the stash entry.

Your local edits come back.

Remote updates remain.

Only if there are conflicts, Git will tell you.

📌 Purpose: Bring back your work after pulling the latest code.




==============================

Create new lxc 
lxc launch ubuntu:22.04 jans-project(name)

check for lxc 
lxc ls

start the lxc
lxc start jans-test

stop the lxc
lxc stop jans-test

go in lxc :- 

lxc exec jans-test bash

Stop lxc

lxc stop ubuntu-containe

Delete lxc 

lxc delete --force jans-test

check file
fl

speed test for net

speedtest-cli

for check the log for cli

-f cli_cmd.log


--> for run lxc url 
open host and write the ip of lxc 
sudo vim /etc/hosts
(add ip) (lxc name)

then open editer
for edit run r
add ip address   10.202.184. mkdocs serve > mkdocs.log 2>&1 &
cat mkdocs.log


Create new lxc 
lxc launch ubuntu:22.04 jans-project(name)

check for lxc 
lxc ls

start the lxc
lxc start jans-test

stop the lxc
lxc stop jans-test

go in lxc :- 

lxc exec jans-test bashchmod 400 ~/Downloads/your-key-file.pem


Stop lxc

lxc stop ubuntu-containe

Delete lxc 

lxc delete --force jans-test

check file
fl

speed test for net

speedtest-cli

for check the log for cli

-f cli_cmd.log


open host and write the ip of lxc 
sudo vim /etc/hosts

then open editer
for edit run r
add ip address   10.202.184.19 jans-test
then apply wq  19 jans-test
then apply wq 




------ tarp auth

when you see the `ok screen then need to check acr value at Auth Server > Authn
if nor avaialve then go to scripts sear that acr value then anable that then you can run the tarp with that acr value.

------
for login 
sudo /opt/jans/jans-cli/jans_cli_tui.py

open host and write the ip of lxc chmod 400 ~/Downloads/your-key-file.pem

sudo vim /etc/hosts

health check  if not able to open tui then run this command two three time 
sudo systemctl list-units --all "jans*"

stop services 
sudo systemctl stop jans-config-api.service

if open editer in lxc 
sudo vim /file-name

edit 
r enter 

without save exit the file 
Press Esc: Ensure you are in command mode by pressing the Esc key. This ensures you are not in insert mode.

Type :q! and Press Enter: This command will force vim to quit without saving any changes.



with save and exit the file 
:wq

create the folder 
Mkdir folder name 

go any folder 

cd folder name 

run any script file 

Execute the Script: Once you're inside the script folder, you can execute the script using its filename preceded by ./ to indicate that it's located in the current directory:

bash
Copy code
./script.sh

   This command will run the script.sh file. Make sure that the script file has execute permissions set. If it doesn't, you can set the execute permission using the chmod command:

 bash
Copy code
chmod +x script.sh




then open editer
for edit run r
add ip address   10.202.184.19 jans-test
then apply wq 



without save exit 

Press Esc: Ensure you are in command mode by pressing the Esc key. This ensures you are not in insert mode.

Type :q! and Press Enter: This command will force vim to quit without saving any changes.




create file 
mkdir script

go in side 
cd script

script.sh

-------
git
git commit 
git commit -S -s -m 'docs: update command header'

go to next state (for commit)
git add docs/admin/install/vm-install/ubuntu.md

git push
git push --set-upstream origin  doc-ubuntu-installation-update

revert commit
  git reset --soft HEAD~
move head on last before commit
git reset --soft HEAD~chmod 400 ~/Downloads/your-key-file.pem


delete the branch 
example 
 ->  git branch -D docs-custom-assets 
need to change branch and keep changes in last branch 
 git stash push -u -m 'openid changes(comment)'
 git stash list
 git stash apply --index
git stash apply stash@{0}



Git letest
 -> git fetch
switech branch 
 -> git switch branch-name(doc-uma-resources)
get branch
 -> git branch -vv

git commit  
    example
 -> git commit -s -m 'fix(docs): update UMA config document'
get commit changes form other branch  3a4088bb= this commint number 
 for get the commit number 
   * git log <branch name> --oneline 
   * you will get number like this :     a08705ac072 (origin/docs-update-readme, docs-update-readme) 
     `a08705ac072` this is number 
get change form other branch 

git cherry-pick -n 3a4088bb(number)


add pach file in project 

 git apply /home/ifour/Downloads/update-cach-configuration-04_06_2024.patch(file name )

get patch
git apply <.patch file>

git log --show-signature 



For run local 

after install the mkdocs need to install tegs 


for local need to run mkdocs 
$ mkdocs serve

for new 
mkdocs serve --dev-addr=localhost:8080

mkdocs list 

pip list | grep mkdocs




link open new tab 
[introspection script](https://github.com/JanssenProject/jans/blob/main/docs/script-catalog/introspection/introspection-role-based-scope/introspection_role_based_scope.py){:target="_blank"}
this for {:target="_blank"}


RUN SCRIPT

sudo vim /script.sh


* In order to successfully create a new `party` entry, users must ensure that both the `Name` and `Domains` fields are populated with the necessary information.

update and upgrade
sudo apt-get update


 sh ~/Documents/lxd-network-script.sh 


run vm 

chmod 600 /home/work/Downloads/private-killdeer.pem
ssh -i /home/work/Downloads/private-killdeer.pem root@198.199.89.32

new
ssh -i /home/work/Downloads/kitten.pem root@68.183.112.240
new
sudo ssh -i /home/work/Downloads/private-key-snipe.pem root@157.230.214.195

impoer the file 
chmod 400 ~/Downloads/your-key-file.pem



set for jans command
nano ~/.bashrc

find gone branch 
git branch -vv | grep ': gone'


ubdo the changes when conflict 
git online

then 
example
git checkout ffb365486f -- docs/janssen-server/developer/scripts/person-authentication.md
work@workstation:~/code/jans$ git checkout ffb365486f -- docs/janssen-server/developer/scripts/update-token.md
work@workstation:~/code/jans$ 



docker
check status 
 sudo docker container ls -a
check avtive
sudo docker container ls
 sudo docker ps
copy id 
stop docker 
 sudo docker stop 11db2b65f3e8
start docker 
sudo docker start 11db2b65f3e8
check log 
sudo docker logs 11db2b65f3e8

go in docker
docker exec -it <container_id_or_name> bash


git diff

git diff (commitnumber)

if you take patch

git diff (commitnumber) > test.patch
npm run dev





===> for run the sbomgr tool

1.make build
2. ./build/sbomgr
run the command 
package name 
./build/sbomgr packages -N 'package name' ./janssbom.json

package name and version 
./build/sbomgr packages -O pkgn,pkgv ./janssbom.json

=> package name and licence 
jq -r '
  .packages[] |
  [.name, (.licenseConcluded // "null")] |
  @tsv
' janssbom.json

null count form sbom
jq '[.packages[] | select(.licenseConcluded == null)] | length' sbom.final.json

=> findout dublicate packages 

jq -r '
  .packages
  | group_by(.name)
  | map(select(length > 1))
  | flatten
  | map([.name, (.licenseConcluded // "null")])
  | .[]
  | @tsv
' sbom.final.json

=> in the dublicate packages filter and keep one 

jq -r '
  .packages
  | group_by(.name)
  | map(select(length > 1))
  | flatten
  | group_by(.name)
  | map({
      name: .[0].name,
      license: (map(.licenseConcluded) | map(select(. != "null")) | .[0] // null)
    })
  | map([.name, (.license // "null")])
  | .[]
  | @tsv
' janssbom.json

==> findout unique packages from sbom

jq -r '
  [.packages[] |
    [.name, (.licenseConcluded // "null")] |
    @tsv
  ] | unique[]' janssbom.json

==> findout unique packages but not unique licence 

jq -r '
  .packages
  | group_by(.name)
  | map(select(length == 1))
  | map({
      name: .[0].name,
      license: (.[0].licenseConcluded // "null")
    })
  | map([.name, .license])
  | .[]
  | @tsv
' testdata.json










==> check the sbom  using parlay
sbome.spdx.json = add your sbom 
sbom.enriched.1.json == will get updated json
parlay ecosystems enrich sbom.spdx.json > sbom.enriched.1.json

parlay install
* add updated version 
  wget https://github.com/snyk/parlay/releases/download/v0.1.4/parlay_Linux_x86_64.tar.gz
* Extract the Binary
  tar -xvf parlay_Linux_x86_64.tar.gz
* Make it Executable
  chmod +x parlay
* Move it to a System Path
  sudo mv parlay /usr/local/bin/



==>  grype
      
      install 
      curl -sSfL https://raw.githubusercontent.com/anchore/grype/main/install.sh | sudo sh -s -- -b /usr/local/bin
       
      test the sbom
      grype sbom:sbom.spdx.json


==> sbomqs

   sudo dpkg -i /home/work/Downloads/sbomqs_1.0.4_amd64.deb 
   
   command 
   sbomqs compliance -f sbom.final.json --color 



-----------------------------------------------------------------------------------------------
lenght of without the licence 
jq '[.packages[] | select(.licenseConcluded == "NOASSERTION" or .licenseConcluded == null)] | length' jans-sbom-18.json

name of without licence package
jq '.packages[] | select(.licenseConcluded == "NOASSERTION" or .licenseConcluded == null) | .name' sbom_updated.json

check score of sbom 
sbomqs score -- sbom_updated.json 





-----------------------------------------------------------------------------------------------


==>  update sbom json add license where not available

#!/bin/bash

CSV_FILE="/home/work/Downloads/parlay-final-sbom.exl.csv"
SBOM_FILE="/home/work/Downloads/jans-sbom.json"
OUTPUT_FILE="sbom_updated.json"

# Run the Python helper inline
python3 - <<EOF
import csv
import json

csv_file = "$CSV_FILE"
json_file = "$SBOM_FILE"
output_file = "$OUTPUT_FILE"

# Step 1: Read CSV into dictionary
csv_data = {}
with open(csv_file, newline='', encoding='utf-8') as f:
    reader = csv.DictReader(f, delimiter='\t')
    for row in reader:
        name = row.get("Package name", "").strip()
        original_license = row.get("License", "").strip()
        if name and original_license:
            csv_data[name.strip()] = original_license.strip()

# Step 2: Load SBOM JSON
with open(json_file, "r", encoding="utf-8") as f:
    sbom = json.load(f)

# Step 3: Update SBOM packages
for pkg in sbom.get("packages", []):
    name = pkg.get("name", "").strip()
    if name in csv_data and "licenseConcluded" not in pkg:
        pkg["licenseConcluded"] = csv_data[name]

# Step 4: Save updated SBOM
with open(output_file, "w", encoding="utf-8") as f:
    json.dump(sbom, f, indent=2)

print(f"✅ Updated SBOM saved to {output_file}")
EOF


for run the script 
chmod +x update_sbom_with_jq.sh
./update_sbom_with_jq.sh


explain script  

1 Create an empty dictionary called csv_data.
2 Read the CSV file:
   * For each row:
     - Take the package name.
     - Check the "Updated" column:
     - If it has data, use it.
     - If it’s empty, use the "License" column instead.

Store this in csv_data like:

```
csv_data["package name"] = "license"
```

3. Read and load the SBOM JSON file into a Python dictionary called `sbom`.

4. Update the SBOM:
 * For every package in sbom["packages"]:
 * If the package does NOT already have a licenseConcluded
 * And the package name exists in csv_data
 * Then: add the license from csv_data into the SBOM under licenseConcluded.

5. Save the updated SBOM to a new file (sbom_updated.json).



--------------------------
database releted



go in db
sudo -i -u postgres


check list 
su - postgres
psql -c "\l"



go in db
psql -d jansdb


table list 
\dt

\x

SELECT * FROM public."jansPerson" LIMIT 10;

UPDATE public."jansPerson"
SET "telephoneNumber" = NULL
WHERE "telephoneNumber" = '7284939479';


UPDATE public."jansPerson"
SET "mobile" = NULL
WHERE "mobile" = '["7284939479"]';
