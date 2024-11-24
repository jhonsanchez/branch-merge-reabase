## Objective
Practice merging techniques (merge vs rebase)

## Exercise

### Merge
- Students fork the repository
- Analyze each branch (commits, files, content)
    ```bash
    # Check main branch
    git switch main
    git log --oneline
  
    # Check lunch branch
    git switch lunch
    git log --oneline
  
    # Check dinner branch
    git switch dinner
    git log --oneline
  
    # Check dessert branch
    git switch dessert
    git log --oneline
    ```
    check all branches at once
    ```bash
    git log --oneline --all --graph
    ```
- Go to main-merge branch
    ```bash
    git switch main-merge
    ```
- Perform a simple merge from the lunch branch
    ```bash
    git merge lunch
    ```
- Review the merge result
- Perform a merge using the `--no-commit` option
    ```bash 
    git merge --no-commit dessert
    ```
- Review the result of the new merge
- What's the difference between the two merges?

### Rebase
- Students fork the repository
- Analyze each branch (commits, files, content)
- Perform a rebase in the dessert branch
    ```bash
    git switch dessert
    git log --oneline
    git rebase main-merge
    ```
- Review the rebase result

## Conclusions
Review results and differences, discuss appropriate scenarios for each case