```sh
git clone git@github.com:angristan/Casper-XYZ.git
cd Casper-XYZ
git remote add upstream https://github.com/TryGhost/Casper.git
git fetch upstream
git merge upstream/master
# Resolve conflicts (accept incoming changes)
yarn install
yarn zip
git add -A
git commit -m "Merge upstream, update to 2.4.0"
git push
```
