# git_commit_template.txt

The idea behind a git commit template is to have a file that helps you write better commits. In order to help you with this we can use a template rather then remembering the rules you have set yourself.

## Where do you put your template?

To make life simple, put it in your home directory as a hidden file (so starting with a `.`). The file name doesn't actually matter but it is handy if you always use the same name in order to be consistent.

## Setting up your global template

To configure git globally, and thus setting your default template you do

```shell
git config --global commit.template ~/.git_commit_template.txt 
```

## Validating your setup

```shell
# making your test environment
mkdir test &&  cd test
git init
touch a
echo "hello world" >> a
git add a
# create your commit
git commit
# cleanup
cd .. && rm test
```

When you type `git commit` you should see your template.
