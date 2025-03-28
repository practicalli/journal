---
title: Neovim updates and Neovide
date: 2023-12-17
authors:
  - practicalli
categories:
  - practicalli
---

Enjoying the new role as there is so much to do that I can get involved with.

Also enjoying Neovide GUI for Neovim, although its more convienient to simply run `astro` for Neovim in a terminal.  When I am comfortable setting the base directory or working with multiple project, then Neovide will be more convienient to use.

<!-- more -->

## Solo ride

Saturday was intended to be a club ride, although I didnt arrive at the starting point in time.  I decided to do the level 3 ride by myself and perhaps catch up to the group.  I did catch up with the group, outside the cafe at the end of the ride.

I did have some minor mechanical issues, so did stop for about 10 minutes.  I also confused the cycling computer for about 5 minutes by taking a wrong turn.  So it seems likely that I would have been able to keep up with the level 3 group if I had arrived earlier.


## Neovim

AstroNvim updates

- [Gist-nvim](https://github.com/Rawnly/gist.nvim) create GitHub Gists from the current buffer (required GitHub CLI - `gh`)
- [GitLinker.nvim](https://github.com/linrongbin16/gitlinker.nvim) generate links for files, including line ranges, for code shared on Git services, e.g. GitHub

Practicalli AstroNvim user configuration updates

- add ignored words configuration for Alex lint tool
- add `set guifont = "Fira Code:h16"` in `options.lua` to set font family and size explicitly for Neovide

Practicalli Neovim

- add install section for MacOSX with Homebrew and from Neovim Release page
- add install page for Neovide


### Conjure update

??? INFO "Conjure recent commit history"
    ```shell
    ○ conjure  clojure
        4880144 Correct janet stdio module form name (9 days ago)
        ec71272 Set __name__ to __repl__ when setting up #540 (13 days ago)
        84a1ba6 Merge branch 'sogaiu-janet-stdio' into develop (13 days ago)
        2dd0976 Swap the nREPL *ns* back to the pre conjure.internal one after setup #539 (13 days ago)
        b9043b6 Default the nREPL Clojure context to user (13 days ago)
        04ade4e Add a little example configuration section #541 (13 days ago)
        02d07de Correct linguist-generated tag for Lua output (13 days ago)
        19c46d5 Support Guile results that lack an assignment (like display) (13 days ago)
        9b027d8 Swap guile dev dir to .nvim.fnl and add display example (13 days ago)
        58da81f Cast lines to string when appending to the log (13 days ago)
        83e5610 Sync sponsors! <3 thank you so much to everyone who supports this, even a tiny bit (13 days ago)
        08834ed Swap the nREPL *ns* back to the pre conjure.internal one after setup #539 (13 days ago)
        e910e33 Default the nREPL Clojure context to user (13 days ago)
        641d263 Add a little example configuration section #541 (13 days ago)
        10e951f Correct linguist-generated tag for Lua output (13 days ago)
        af8a3da Support Guile results that lack an assignment (like display) (2 weeks ago)
        befd4e7 Swap guile dev dir to .nvim.fnl and add display example (2 weeks ago)
        6c70271 Cast lines to string when appending to the log (2 weeks ago)
        ba21ef7 Sync sponsors! <3 thank you so much to everyone who supports this, even a tiny bit (2 weeks ago)
        5036ec7 Add a stdio based janet client (7 weeks ago)
        cb86d46 Only send the Conjure client name once the Janet/netrepl REPL is connected #532 (8 weeks ago)
        d687f52 Don't set the conn in the janet state until it's connected (8 weeks ago)
        2eb9682 Integrate #mapping#enable_defaults into every client (8 weeks ago)
        79d54e4 Apply mapping#enable_defaults to clojure (8 weeks ago)
        e37e9f2 Compile config.lua, remove a print (8 weeks ago)
        fbdcd9b Add a g:conjure#mapping#enable_defaults flag which keeps the mapping code but removes the defaults #533 (8 weeks ago)
        2df49cb Apply patch to janet from #532, fixing paths on Windows (8 weeks ago)
        28b61dc Sync sponsors (tyvm @axvr!) (8 weeks ago)
        bf5a393 Make HUD zindex configurable and default to 1 (was 10) (10 weeks ago)
     ```

??? INFO "Neogit commit updates"
    ```shell
    ○ neogit  User AstroGitFile  <leader>gnk  <leader>gs  <leader>gnt  <leader>gnc  <leader>gnd
        49755ff Merge pull request #1043 from NeogitOrg/fix/popup-mappings (17 minutes ago)
        c6cb986 Use nil check instead of metatable. (19 minutes ago)
        69fb64c Merge pull request #1039 from ttytm/fix/abort (3 hours ago)
        4221b79 Merge pull request #1040 from ttytm/fix/type-defs (3 hours ago)
        41281bc Fix type definitions (4 hours ago)
        7ecf75a Fix close abort (4 hours ago)
        a6a7ec0 Update README.md (7 hours ago)
        6ae788e Merge pull request #1038 from NeogitOrg/upgrade/editor-commands (8 hours ago)
        da7c378 Breaking! Remove option `disable_commit_confirmation`. You can now just use a dedicated "Submit" and "Abort" action if you don't want a confirmation. (8 hours ago)
        6bdff60 Ensure all editors have same filesystem layout (8 hours ago)
        a33a691 Add config for commit_editor mappings (8 hours ago)
        362c7a9 Ensure on_unload callback is called the same thing in all editors (8 hours ago)
        d171ca9 Rework how commit editor handles closing/saving/aborting (8 hours ago)
        0932542 Merge pull request #1033 from NeogitOrg/mappable-rebase-keys (9 hours ago)
        1990f97 cleanup (9 hours ago)
        6a75ae9 Set metatable to handle NOP keys (10 hours ago)
        86ad252 Lint (21 hours ago)
        f02f3d7 Merge pull request #1036 from NeogitOrg/fix/branch/revision (21 hours ago)
        1207e96 Fix: Can't prefix heads/, remotes/, tags/ and expect things to work (21 hours ago)
        b14b86e When doing interactive rebase, and aborting, don't show a scary message. Be nicer. (22 hours ago)
        2e5f285 Validate rebase editor mappings (22 hours ago)
        7860697 Add help message in rebase buffer (22 hours ago)
        c2b7493 Use norm! to prevent issues with user maps (22 hours ago)
        385aac7 Remove comment - only return the changed string, not number of changes here (22 hours ago)
        ee80acd Pull in max_length util function (22 hours ago)
        473a79b Lint (2 days ago)
        dbf457c Use user mappings for rebase editor; add moveup, movedown, submit, abort (2 days ago)
        9224a1a Add rebase editor commands to config for user mappings (2 days ago)
        0ae5548 Neogit.client can now exit(1) to signify an aborted commit. (2 days ago)
        1177aaa Use buffer:write (2 days ago)
        29c5c58 Add buffer:write method (2 days ago)
        d6f21d8 Merge pull request #1030 from gollth/remote-popup (2 days ago)
        0917973 Remote Popups in {Commit, Log, Reflog} Views (2 days ago)
        a13aa47 Merge pull request #1026 from NeogitOrg/fix/reset-to-tags (3 days ago)
        7b86103 Allow resetting to tags, and use full ref names to prevent colission between tags/branches with same name. (3 days ago)
        92b3a3c Merge pull request #1025 from NeogitOrg/checkout-tags (3 days ago)
        7a96186 Allow checking out tags from b b (3 days ago)
        a74a25e Merge pull request #1022 from NeogitOrg/CKolkey-patch-1 (3 days ago)
        8f38d8f Merge pull request #1023 from NeogitOrg/enhancement/filter-commit-diffs (3 days ago)
        be7751a lint (3 days ago)
        932ee81 Pass item filter into log view, so it can be used to filter commits opened, so they only show diff's for filtered files. (3 days ago)
        b0dd97f Remove notification from commit view init (3 days ago)
        4f5b7bd Update README.md (3 days ago)
        7782058 Merge pull request #1021 from NeogitOrg/fix/auto-fetch-remotes (3 days ago)
        8956302 Merge branch 'master' into fix/auto-fetch-remotes (3 days ago)
        735d618 When fetching after checkout, repo state isn't updated. Need to check upstream manually. (3 days ago)
        a2361d2 Merge pull request #810 from NeogitOrg/auto-fetch-remotes (4 days ago)
        275451a Update config.lua (4 days ago)
        86636d0 Set default for fetch_after_checkout to false for now (4 days ago)
        d7990c3 Merge pull request #1012 from NeogitOrg/fixup/log (4 days ago)
        17eb869 Merge pull request #1013 from NeogitOrg/enhancement/rebase-buffer (4 days ago)
        568cbcb Fix tests (4 days ago)
        857c948 Capture OID more robustly (4 days ago)
        06e3ee8 Add documentation for rebase todo commands (4 days ago)
        54dd6fb Add commands to rebase buffer (4 days ago)
        066f92a Allow specifying 'kind' for commit buffer (4 days ago)
        657c13d Reorder log popup switches, and use '-' instead of '=' (4 days ago)
        38a62b3 Merge pull request #1011 from NeogitOrg/fix/rebase-root (4 days ago)
        98d3064 Lint comment (4 days ago)
        232c105 Needed for rebase (4 days ago)
        08a8b5e Hide git remote calls (4 days ago)
        c9156f6 When --root argument is passed to git.rebase.interactively, remove the commit hash from the command. (4 days ago)
        0cdc73e Merge pull request #1010 from NeogitOrg/delete-notification-message (5 days ago)
        8d0a596 Delete notification message after it's done (5 days ago)
        9e3c959 Merge pull request #1009 from NeogitOrg/CKolkey-patch-1 (5 days ago)
        d0424cf Update README.md (5 days ago)
        cebebcd Merge pull request #1008 from NeogitOrg/fix/git-command-history (6 days ago)
        e2d5ba0 Stdout, then stderr (6 days ago)
        58c11c6 Always show error for interactive commands (6 days ago)
        a1afd4a Make failed process warnings easier to read (6 days ago)
        748adcf Always show both stdout and stderr in git command history (6 days ago)
        d391a07 Merge branch 'master' into auto-fetch-remotes (6 days ago)
        6be6676 Merge pull request #1007 from NeogitOrg/fix/selene-CI (6 days ago)
        6844b3e empty (6 days ago)
        81ec2d5 Add stylua version (6 days ago)
        badc33c Change cache (6 days ago)
        cd6bf5c test push (6 days ago)
        946b65b ENV, not OUTPUT (6 days ago)
        4e7fcfd fix cache key (6 days ago)
        2f4b5d3 Use up-to-date rust toolchain (6 days ago)
        2f8e06c Store env var (6 days ago)
        ca75650 modify selene save set (6 days ago)
        f3953df Merge pull request #1006 from NeogitOrg/fix/watcher-scheduler (6 days ago)
        6e034cf Call scheduler first so the cli call doesn't crash when invoked via watcher (6 days ago)
        8ff18e2 Use new error api (6 days ago)
        32ed239 Merge branch 'master' into auto-fetch-remotes (6 days ago)
        37d5d9f Merge pull request #1005 from NeogitOrg/async-refresh-2 (6 days ago)
        443ad6b Move cursor restoration logic to after fn (6 days ago)
        cf97109 cleanup (6 days ago)
        110b8ac Wait on status to finish refreshing (6 days ago)
        59d7680 Reimplement partial refreshing (6 days ago)
        bebb153 Pass nil when partial refreshing doesn't apply (6 days ago)
        9fbc8b4 Rewrite repo to use callback when refreshing. Removes partial refreshing for now (6 days ago)
        92d7ecb Use callback when rendering status buffer - restore cursor location in callback, if it was stored (6 days ago)
        857adae Merge pull request #1004 from NeogitOrg/actions-api-internal-args (8 days ago)
        7ac1e3d Merge branch 'master' into actions-api-internal-args (8 days ago)
        506f14a lint (8 days ago)
        4a5cc7e Pause watcher while executing action (8 days ago)
        68ed281 Don't refresh for these little files (8 days ago)
        47e7dd3 Remove debounce from watcher - this would mess up the semaphore locking the status buffer from repainting. (8 days ago)
        11f6840 Polish (8 days ago)
        9686ce1 Hide this too (8 days ago)
        225902e Revert 1 commits (8 days ago)
        e0296cb comment out watcher (revert me) (8 days ago)
        0ddf77d Hide fs-tree calls (8 days ago)
        481a866 Hide rev-parse calls (8 days ago)
        f4877cb Status is always needed, so call it here (8 days ago)
        541724a Include branch lib (8 days ago)
        5811135 Remove comment (8 days ago)
        3961d73 Format (8 days ago)
        1ed5062 Move branch refresh into branch lib (8 days ago)
        dbf9271 Use loop instead of fn (8 days ago)
        c84894d Use cli (8 days ago)
        761e9be Merge pull request #1003 from NeogitOrg/actions-api-internal-args (8 days ago)
        ffe9295 Change remove_item_from_table to return true if it removed the item(s) (8 days ago)
        3ad0f61 Add support for internal args to .action() api (8 days ago)
        6d445e4 Merge pull request #1000 from NeogitOrg/fix/on-error-for-new-repo (9 days ago)
        ead172f Fix on_error when opening in a non-git directory (9 days ago)
        d0ed65e Merge pull request #880 from NeogitOrg/Expand-default-args (9 days ago)
        34de2a2 No reason to call this over and over, it's always the same thing (9 days ago)
        a1fec2e Merge branch 'master' into Expand-default-args (9 days ago)
        3488b9c Merge pull request #998 from NeogitOrg/fix/dont-trim-commit (9 days ago)
        c20d795 Allow opting out of trimming stdout (9 days ago)
        8b9bd5c Escape properly (9 days ago)
        547bea3 Revert 1 commits (9 days ago)
        d9abf38 Fix bug in pattern escape: need to handle %'s before anything else (9 days ago)
        5828770 This is a default setting (9 days ago)
        5628fb4 Use pattern escape for string (9 days ago)
        3191500 Merge branch 'master' into Expand-default-args (10 days ago)
        dd288fa Merge pull request #967 from NeogitOrg/hide-from-git-history (10 days ago)
        f32d186 Hide more things and lint (10 days ago)
        5f1c7b7 Fix process spec (10 days ago)
        10dadd9 Change log level from error to warn (10 days ago)
        4048119 Lint (10 days ago)
        5133b1c Simplify error handling - always pass callback (10 days ago)
        34d80e3 Centralize calling of :trim() (10 days ago)
        e024521 Don't double notify on error (10 days ago)
        5a1eced Rename "ignore_code" to "ignore_error" (10 days ago)
        ec9aa05 Merge branch 'master' into hide-from-git-history (10 days ago)
        0b5876c Merge pull request #997 from NeogitOrg/cleanup/parallel (10 days ago)
        f4fba7c Remove unused require (10 days ago)
        48ca87f Remove unused "job" code (10 days ago)
        f94beff Remove unused "parallel builder" code (10 days ago)
        03c278b Merge pull request #995 from NeogitOrg/fix/status-refreshing (10 days ago)
        cbfb897 Nil check buffer (10 days ago)
        987eeda Don't need CLI (10 days ago)
        245f882 Merge branch 'master' into fix/status-refreshing (10 days ago)
        3ac3215 Merge pull request #996 from NeogitOrg/fix/cursor-placement-in-status (10 days ago)
        8364cca Log watcher as refresh source (10 days ago)
        2d55cf1 Cleanup status refresh logic (10 days ago)
        b3c0446 Use vim.api instead of vim.fn to set cursor position (10 days ago)
        e0b9687 Merge pull request #993 from NeogitOrg/fix/reschedule (11 days ago)
        40f4ec4 Need to schedule here - breaks when opening commit editor otherwise (11 days ago)
        62cc708 Merge pull request #875 from NeogitOrg/fix/restore-cursor-location (11 days ago)
        ade6dc5 Merge branch 'master' into fix/restore-cursor-location (11 days ago)
        119b4fb Merge pull request #930 from GCBallesteros/add-commit-navigation (11 days ago)
        15bf3f9 Merge branch 'master' into hide-from-git-history (12 days ago)
        f59b0e9 Merge pull request #992 from NeogitOrg/rebase-a-subset (12 days ago)
        66e31fb Add git rebase --edit-todo command to rebase popup (12 days ago)
        7abd392 Fix rebase popup rebase-merge options (12 days ago)
        8ef9780 notes (12 days ago)
        e855762 Expand branch docs (12 days ago)
        e21c391 Add rebase popup help (12 days ago)
        daa7b9f Merge pull request #991 from NeogitOrg/fix/missing-status-hint-mappings (12 days ago)
        6cbed41 Check both status and popup maps for hints (12 days ago)
        9dce695 Cleanup rebase module (2 weeks ago)
        d12bc48 Rename rebase onto lib function (2 weeks ago)
        1accbba Add action: Rebase Subset (2 weeks ago)
        468f545 lint (3 weeks ago)
        539e78f Add default opts (3 weeks ago)
        7035226 Added another arg (3 weeks ago)
        5515206 Merge branch 'master' into hide-from-git-history (3 weeks ago)
        22e4322 Lint (3 weeks ago)
        d03f81b Hide all calls in git.files lib (3 weeks ago)
        b20bd95 Hide more background calls. (3 weeks ago)
        cde49bb Replace builder style call with an option passed into call() or call_sync() (3 weeks ago)
        3b2f5aa Pass opts to call() and call_sync() - replace "ignoring_exit_code" with option on call/call_sync (3 weeks ago)
        4ce821b lint (3 weeks ago)
        d08d723 Update cli lib to allow hiding cli commands executed from git history buffer (3 weeks ago)
        fbf5fa8 Hide some internal state building commands from displayed git history (3 weeks ago)
        3c52bb1 Allow git.log.list() to be called but hidden, since it's used for some internal state building (3 weeks ago)
        7b99857 Move constants up a scope (3 weeks ago)
        243b712 Filter hidden git commands from history buffer (3 weeks ago)
        f3668de Remove unused code for "parallel builder" (3 weeks ago)
        2ecb1a8 Cleanup (3 weeks ago)
        a6f363d Use direct CLI call here so we don't stack too much behaviour (3 weeks ago)
        287abae Merge branch 'master' into auto-fetch-remotes (3 weeks ago)
        63c3738 Feat: Jump to file with `<CR>` on the CommitView (5 weeks ago)
        7756191 Expand default args to match Magit (experiment) (10 weeks ago)
        31f24cb Formatting (2 months ago)
        758d263 These don't seem to do anything (2 months ago)
        75e4085 Properly store/restore cursor location. It seems that close() gets called twice, so put in a lockout to prevent that. (2 months ago)
        806267c Auto-fetch functions (3 months ago)
        328bb3e Extract to git lib (3 months ago)
        b6bed92 Add config (3 months ago)
    ```

---
Thank you.

[:globe_with_meridians: Practical.li Website](https://practical.li){target=_blank .md-button}

[:fontawesome-brands-github: Practical.li GitHub Org](https://github.com/practicalli){target=_blank .md-button}
[:fontawesome-brands-github: practicalli-johnny profile](https://github.com/practicalli-johnny){target=_blank .md-button}

[:fontawesome-brands-mastodon: @practicalli@clj.social](https://clj.social/@practicalli){target=_blank .md-button}
[:fontawesome-brands-twitter: @practical_li](https://twitter.com/practcial_li){target=_blank .md-button}
