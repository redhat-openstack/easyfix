
## Hacking

oneline for cloning a bunch of dist-git repos to local machine

(Credits to snecklifter)

curl -s https://api.github.com/orgs/rdo-packages/repos?per_page=100 | ruby -rubygems -e 'require "json"; JSON.load(STDIN.read).each { |repo| %x[git clone #{repo["ssh_url"]} ]}'

