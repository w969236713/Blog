```text
set easymotion
set surround
set multiple-cursors
set nu
set rnu
set clipboard=unnamed,autoselect
set hlsearch
set incsearch
set scrolloff=2
set ignorecase
set smartcase
set showmode
set history=10000
set NERDTree

let mapleader = " "
let g:mapleader = " "



" 重新载入ideavimrc
nnoremap <leader>r <ESC>:source ~/.ideavimrc<CR>


"设置快捷移动 easy motion"
map , <Plug>(easymotion-prefix)


"Turn on case insensitive feature
let g:EasyMotion_smartcase = 1
"Use upper target labels and type as a lower case
let g:EasyMotion_use_upper = 0


" move to character
nmap f <Plug>(easymotion-s2)
xmap f <Plug>(easymotion-s2)
omap f <Plug>(easymotion-s2)
" move to word
nmap F <Plug>(easymotion-bd-w)
xmap F <Plug>(easymotion-bd-w)
omap F <Plug>(easymotion-bd-w)

map <Leader>l <Plug>(easymotion-lineforward)
map <Leader>j <Plug>(easymotion-j)
map <Leader>k <Plug>(easymotion-k)
map <Leader>h <Plug>(easymotion-linebackward)

let g:EasyMotion_startofline = 0 " keep cursor column when JK motion


"设置目录树
nnoremap tt <ESC>:NERDTreeToggle<CR>
nnoremap tf <ESC>:NERDTreeFind<CR>







" general
nnoremap <Leader>g :<C-u>action FindInPath<CR>
nnoremap <Leader>r :<C-u>action RenameElement<CR>
nnoremap <Leader>o :<C-u>action RecentProjectListGroup<CR>
nnoremap <Leader>d :<C-u>action ChooseDebugConfiguration<CR>
nnoremap <Leader>w :<C-u>action CloseAllEditorsButActive<CR>
nnoremap <Leader>e :action SearchEverywhere<cr>
nnoremap <Leader>E :action Switcher<cr>
nnoremap <Leader>q :action CloseContent<cr>
nnoremap <Leader>w :action CloseContent<cr>
nnoremap <Leader>Q :action ReopenClosedTab<cr>
nnoremap <Leader>t :action FileStructurePopup<cr>
nnoremap <Leader>a :action Annotate<cr>
nnoremap <Leader>b :action ToggleLineBreakpoint<cr>
nnoremap <Leader>u :action FindUsages<cr>
nnoremap <leader>T :action GotoSymbol<cr>

" Redo
nnoremap U <C-r>

" go to somewhere (g in normal mode for goto somewhere)
nnoremap ga :<C-u>action GotoAction<CR>
nnoremap gc :<C-u>action GotoClass<CR>
nnoremap gd :<C-u>action GotoDeclaration<CR>
nnoremap gs :<C-u>action GotoSuperMethod<CR>
nnoremap gi :<C-u>action GotoImplementation<CR>
nnoremap gf :<C-u>action GotoFile<CR>
nnoremap gm :<C-u>action GotoSymbol<CR>
nnoremap gl :<C-u>action JumpToLastChange<CR>
nnoremap gu :<C-u>action ShowUsages<CR>
nnoremap gt :<C-u>action GotoTest<CR>
nnoremap gp :<C-u>action FindInPath<CR>
nnoremap gr :<C-u>action RecentFiles<CR>
"nnoremap gh :<C-u>action Back<CR>
"nnoremap gl :<C-u>action Forward<CR>

" code editing
"nnoremap == :<C-u>action ReformatCode<CR>
"vnoremap == :<C-u>action ReformatCode<CR>
" nnoremap \i :<C-u>action OptimizeImports<CR>
" vnoremap \i :<C-u>action OptimizeImports<CR>
" nnoremap \r :<C-u>action RenameElement<CR>
nnoremap q :<C-u>action ShowIntentionActions<CR>
"注释



" Ctrl+Shift+Tab Ctrl+Tab
nnoremap <c-s-tab> gT
nnoremap <c-tab> gt

" clear the search buffer when hitting return
nnoremap <space><cr> :nohlsearch<cr>


" options
nnoremap cow :action EditorToggleUseSoftWraps<cr>
nnoremap col :action EditorToggleShowWhitespaces<cr>
nnoremap ta :action Annotate<cr>
nnoremap tb :action ToggleLineBreakpoint<cr>
nnoremap tm :action ToggleBookmark<cr>



nnoremap tm :action ToggleBookmark<cr>

" Run and debug
nnoremap \r :action RunClass<cr>
nnoremap \R :action Run<cr>
nnoremap \d :action DebugClass<cr>
nnoremap \D :action Debug<cr>
nnoremap \c :action CheckStyleCurrentFileAction<cr>

" unimpaired mappings
nnoremap [<space> O<esc>j
nnoremap ]<space> o<esc>k
nnoremap [q :action PreviousOccurrence<cr>
nnoremap ]q :action NextOccurrence<cr>
nnoremap [m :action MethodUp<cr>
nnoremap ]m :action MethodDown<cr>
nnoremap [c :action VcsShowPrevChangeMarker<cr>
nnoremap ]c :action VcsShowNextChangeMarker<cr>


" built-in navigation to navigated items works better
" nnoremap <c-o> :action Back<cr>
" nnoremap <c-i> :action Forward<cr>
" but preserve ideavim defaults
nnoremap g<c-o> <c-o>
nnoremap g<c-i> <c-i>

" built in search looks better
" nnoremap / :action Find<cr>
" but preserve ideavim search
noremap ' <ESC>:action Replace<cr>
"noremap g' <ESC>:action ReplaceInPath<cr>

nnoremap [[ :action MethodUp<cr>
nnoremap ]] :action MethodDown<cr>








```
