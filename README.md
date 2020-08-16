## 7 Most Featured CSS Layouts
### This is inspired my Google Chrome Developers
[Youtube Video](https://www.youtube.com/watch?v=qm0IfG1GyZU&t=269s)

### Check out live-site for this simple project!
[See Live Site](https://bundy-mundi.github.io/css-layouts/)

### #1 Super Centered
    .super-centered{
      display: grid;
      place-items: center;
    }
### #2 The Deconstructed Pancake
    .deconstructed-pancake-parent{
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      box-shadow: 0px 0px 2px 2px rgba(50, 50, 50, 0.75);
    }
    .deconstructed-pancake-children-stretched{
      flex: 1 1 150px; /* Shrinks until the boxes reaches 150px */
      margin: 5px;
      height: auto;
    }
    .deconstructed-pancake-children-non-stretched{
      flex: 0 1 150px; /* No Stretching, determines each box's width and breakpoints */
      margin: 5px;
      height: auto;
    }

### #3 Sidebar Says
    .sidebar-parent{
      display: grid;
      grid-template-columns: minmax(150px, 25%) 1fr;
    }
    .sidebar-children{
      padding: 2rem;
      font-size: 1.2rem;
    }

### #4 Pancake Stack
    .pancake-stack-parent{
      display: grid;
      grid-template-rows: auto 1fr auto;
    }
    .pancake-stack-children{
      padding: 2rem;
    }


### #5 Classic Holy Grail Layout
    .classic-parent{
      display: grid;
      grid-template: auto 1fr auto / auto 1fr auto;
    }
    .classic-children{
      padding: 2rem;
    }
    .header{
      grid-column: 1 / 4;
    }
    .footer{
      grid-column: 1 / 4;
    }
    .left-sidebar{
      grid-column: 1 / 2;
    }
    .right-sidebar{
      grid-column: 3 / 4;
    }

### #6 RAM(Repeat, Auto, Minmax)
    .ram-parent{
      display: grid;
      grid-gap: 1rem;
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      padding: 1rem;
      box-shadow: 0px 0px 2px 2px rgba(50, 50, 50, 0.75);
    }
    .ram-children{
      font-size: 1.2rem;
    }

### #7 Clamping My Style
    .clamping-parent{
      display: grid;
      place-items: center;
      box-shadow: 0px 0px 2px 2px rgba(50, 50, 50, 0.75);
    }
    .clamping-card{
      padding: 1rem;
      width: clamp(20rem, 50%, 30rem);
      display: flex;
      flex-direction: column;
      justify-content: center;
      background-color: antiquewhite;
      border-radius: 2px;
    }