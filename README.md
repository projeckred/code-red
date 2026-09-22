# code-red — Shared Resources

Repository for R.ED's introductory coding programme, where students apply programming fundamentals by building games with Scratch or Greenfoot.

## Structure

Each group has its own folder under `groups/`, containing their game project
in either Scratch or Greenfoot.

groups/
├── group-01/Scratch/game.sb3
├── group-02/Greenfoot/my-game-project/
└── ...

## Branching guide — for the participating groups

Each group works on their own branch from `main`. `main` only ever holds the
shared templates, resources, and docs — never a group's actual game files.

**1. Create your branch**

```bash
git checkout main
git pull
git checkout -b group-01
```

Use `group-01` through `group-10`, matching your group number.

**2. Work inside your group folder**

Add your project files under your group's folder, using the game engine you choose:

groups/group-01/Scratch/game.sb3

or

groups/group-02/Greenfoot/my-game-project/


**3. Commit and push your branch**

```bash
git add .
git commit -m "Group 01: add Scratch game"
git push -u origin group-01
```

**4. Keep committing as you build**

```bash
git add .
git commit -m "Group 01: add scoring logic"
git push
```

**5. (Optional) Share your finished game**

Open a pull request from your branch (`group-01`) into `main` once your game
is ready, so it appears in the final shared repo.

**Rule of thumb:** only touch files inside your own `groups/group-XX/` folder — this avoids merge conflicts with other groups.