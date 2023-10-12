

### 1. Git Backup settings

#### Automatic

- **Split automatic commit and push**：这个选项可以让你独立地设置提交(commit)和推送(push)的定时器。如果启用，你可以分别设置两者的时间间隔。对于频繁的修改，建议先提交再稍后推送。
    
    英文：Enable to use separate timer for commit and push
    
- **Vault backup interval (minutes)**：设置自动提交和推送的时间间隔。例如，如果设置为10，则每10分钟自动保存和上传更改。
    
    英文：Commit and push changes every X minutes. Set to 0 (default) to disable.
    
- **Auto Backup after stop editing any file**：编辑任何文件后，是否立即自动备份。这可以确保你每次编辑完文件后都有一个备份。
    
    英文：Requires the backup interval not to be 0. If turned on, do auto backup every 0 minutes after stop editing any file. This also prevents auto backup while editing a file.
    
- **Auto backup after latest commit**：是否在最近一次提交后自动备份。
    
    英文：If turned on, set last auto backup time to latest commit
    
- **Auto pull interval (minutes)**：设置自动从远程仓库拉取(pull)的时间间隔。
    
    英文：Pull changes every X minutes. Set to 0 (default) to disable.
    
- **Specify custom commit message on auto backup**：启用此选项可以为自动备份设置自定义提交信息。
    
    英文：You will get a pop up to specify your message
    

### 2. Commit message

- **Commit message on manual backup/commit**：手动备份/提交时使用的提交信息。这里可以使用占位符，例如`{date}`会被替换为当前日期和时间。
    
    英文：Available placeholders: `{date}`, `{hostname}`, `{numFiles}`, and `{files}`
    

### 3. Backup

- **Sync Method**：选择用于处理新更改的方法。建议使用默认的"Merge"。
    
    英文：Selects the method used for handling new changes found in your remote git repository.
    
- **Pull updates on startup**：当Obsidian启动时，是否自动从远程仓库拉取更新。
    
    英文：Automatically pull updates when Obsidian starts
    
- **Push on backup**：备份时是否推送到远程仓库。如果关闭，只会保存更改，不会上传。
    
    英文：Disable to only commit changes
    
- **Pull changes before push**：在推送之前是否先拉取更改。
    
    英文：Commit -> pull -> push (Only if pushing is enabled)
    

### 4. Line author information

- **Show commit authoring information next to each line**：在每一行旁边显示提交的作者信息。
    
    英文：Show commit authoring information next to each line
    

### 5. Miscellaneous

- **Automatically refresh Source Control View on file changes**：文件更改后是否自动刷新源代码控制视图。
    
    英文：Automatically refresh Source Control View on file changes
    
- **Source Control View refresh interval**：刷新源代码控制视图的时间间隔。
    
    英文：Milliseconds to wait after file change before refreshing the Source Control View
    
- **Disable notifications**：是否禁用关于git操作的通知。
    
    英文：Disable notifications for git operations to minimize distraction