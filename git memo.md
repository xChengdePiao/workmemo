- 元に戻す時  
	` git rm --cached -r .`  
	` git reset --hard `

- 直前のコミットをなかった事にする（@はHEADのエイリアス）  
	` git reset --hard HEAD^  `  
	` git reset --hard @^  `

- n個前のコミットに戻る  
	` git reset --hard HEAD~{n}`  
	` git reset --hard @~{n}`

- 最後のコミットを直す  
	`git commit --amend   `  
	`git commit --amend -m "some comment"`

- 最新のｎ個のログ、diffを取得  
	`	git log -p -2	`

- 最新のみ取得  
	`git clone --depth 1 https://github.com/git/git	`

- 作業を一時退避  
	`git stash`

- stashされたリストを見る  
	`git stash list`

- 最後に退避した変更を適用する  
	`git stash apply`

- 退避した変更指定して適用する  
	`git stash apply stash@{2}`

- 退避した変更を削除  
	`git stash drop stash@{2}`
