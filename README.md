# GuideLines
## Commits Style Guidelines

#### Commit Types

The commit title consists of the type of the message and subject. The type is contained within the title and can be one of these types:
Emojies should be unique per developer 

Emoji + TAG + Commit subject 

* **[INIT]** creating a new project, initial commit
* **[FIX]** fix a bug
* **[IMPL]** code update with new tasks etc.
* **[REFACTOR]** code refactoring


#### Commit Subject 

Subjects should be no greater than approx 50 characters, should have capitalized first character.

Use an imperative tone to describe what a commit does, rather than what it did. 
Examples, 

```bash
🧸 [INIT] Inital commit
🌙 [IMPL] Firebase implementation
⚡️ [BUGFIX] Notification bug fixed
🍉 [REFACTOR] Address detail new structure integrated
```

## Branch Strategy 
All main branches or task branches should be create from development branch. 

If you need package of some tasks(not all tasks) for testing,regression etc. you should create another branch like main branch and create pull requests for them. In the normal scenario you will be merge all branch PR to main branch after that main branch PR to development branch.

If you create critical fix for everyone or another tasks connected your component development, you can create PR directly to development branch. 
And then you need to report this to your teammates

Master  Branch is a release branch

```bash
-Development 
-Master 
-v1.0.0
  -main
  -[TaskID]-[TaskSubject]
-v1.0.1
  -main
  -[TaskID]-[TaskSubject]  
```
