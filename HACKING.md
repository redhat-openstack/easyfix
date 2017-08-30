
## Hacking

script for cloning a bunch of dist-git repos to local machine

(Credits to https://gist.github.com/michfield/4525251)

```
url="https://api.github.com/orgs/rdo-packages/repos";
num=$(curl -sI "$url?page=1&per_page=100" | sed -nr 's/^Link:.*page=([0-9]+)&per_page=100>; rel="last".*/\1/p');
for ((i=1;i<=$num;i++)); do ( curl -s "$url?page=${i}&per_page=100" | grep "clone_url" | sed -nr 's/.*clone_url": "(.*)",/git clone \1/p' ); done >clone_all_repos.sh

```

Then chmod +x and run the resulting script

You might need to specify the branch, e.g.

git clone https://github.com/rdo-packages/nova-distgit.git --branch rpm-master
