Template for composer packages (PHP 7.2 legacy edition)
=======================================================

**Quick start:**
```
NEW_REPOSITORY_NAME=FOOBAR; \
git clone https://github.com/ebln/template-php-package-7.2.git ${NEW_REPOSITORY_NAME} && cd ${NEW_REPOSITORY_NAME}

git remote set-url origin git@github.com-ebln:ebln/${NEW_REPOSITORY_NAME}.git
git push --set-upstream origin master
```

## Consider

* Is this public, incognito or private
    
* [Review and edit composer.json](composer.json)
    * author
    * autoload namespace
    * name, description, keywords
    * [license](https://help.github.com/articles/licensing-a-repository/#searching-github-by-license-type)
    * requirements: versions still valid?

* Update this README.md file!
    
* [Choose](https://choosealicense.com/) a [license](LICENSE)
    
* [Review and edit .gitignore](.gitignore)  

## Setup
* Clone this boilerplate
    * ```bash
      NEW_PROJECT_NAME=FOOBAR; \
      git clone https://github.com/ebln/template-php-package-7.2.git ${NEW_PROJECT_NAME} && cd ${NEW_PROJECT_NAME}  
      ```
* Setup git
    * Create a new (origin) repository
        * Define its name as a variable: `export REPOSITORY_NAME=FOOBAR;`
    * Option: *start all over*
        1. `rm -rf .git && git init` # to flush boilerplate's git history
        2. Configure git for your privacy demands
            ```bash
            git remote remove origin; \
            git config --list; \
            git config user.email "sokolow@net.invalid"; \
            git config user.name "Распутин"; \
            git config --list --show-origin;
            ```
        3. Add origin
            ```bash
              git remote add origin git@github.com-ebln:ebln/${REPOSITORY_NAME}.git
            ```
        4. as this is a new repository, run: ``
            ```bash
                git add -A && git commit -m 'Initial commit'
            ```
    * Option: *keep the history from the template*
        * Update origin
          ```bash
            git remote set-url origin git@github.com-ebln:ebln/${REPOSITORY_NAME}.git
          ```
* Set upstream & push
    ```bash
    git push --set-upstream origin master
    ```

