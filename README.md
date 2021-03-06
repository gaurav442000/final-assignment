<html>
    <head>
        
            <meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1.0">
            <meta http-equiv="X-UA-Compatible" content="ie=edge">
            <title>Trello Board</title>
            <link rel="stylesheet" href="external/reset.css">
            <link rel="stylesheet" href="css/utils.css">
            <link rel="stylesheet" href="css/trello-dashboard.css">
            <link rel="stylesheet" href="css/trello-board.css">
            <!--
                Downloaded from https://fontawesome.com/how-to-use/on-the-web/setup/hosting-font-awesome-yourself
            -->
            <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.11.2/css/all.min.css">
        
        <title>Final Assignment</title>
        <style>
            .navbar {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    display: flex;
    justify-content: space-between;
    height: 50px;
    padding: 8px 20px;
    background-color: rgba( 64, 144, 172, 0.65 );
    color: white;
}

.navbar .menu {
    justify-content: flex-start;
}
.navbar > * {
    width: 300px;
    display: flex;
    flex-direction: row;
    align-items: center;
}
ol, ul {
    list-style: none;
}
.navbar .menu > *, .navbar .actions > * {
    display: inline-block;
    padding: 8px;
    border-radius: 2px;
    margin: 0px 4px;
    background-color: rgba( 64, 144, 172, 1 );
}
.pointer {
    cursor: pointer !important;
}

.fa, .fas {
    font-weight: 900;
}
.fa, .far, .fas {
    font-family: "Font Awesome 5 Free";
}
.fa, .fab, .fad, .fal, .far, .fas {
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    display: inline-block;
    font-style: normal;
    font-variant: normal;
    text-rendering: auto;
    line-height: 1;
}

.fa-home::before {

content: "\f015";

}
.navbar .menu-input {
    background-color: transparent;
    padding: 0;
}
.navbar .menu > *, .navbar .actions > * {
    display: inline-block;
    padding: 8px;
    border-radius: 2px;
    margin: 0px 4px;
    background-color: rgba( 64, 144, 172, 1 );
}

.navbar .menu-input input {
    width: 120px;
    padding: 4px 0.5em;
    border: none;
    border-radius: 2px;
    outline: none;
    background-color: rgba( 64, 144, 172, 1 );
    color: white;
    font-size: 1.15em;
    line-height: 1.4;
    color: black;
}
.navbar .menu-input input:focus {
    background-color: white;

}

.task-list .task, .task-list input, .task-list textarea, .task-list button {
    border-radius: 4px;
}
.pointer:hover {
    opacity: 0.7;
}
.task {
    padding: 10px;
    margin: 10px 0;
    background-color: white;
}
.pointer {
    cursor: pointer !important;
}

.task:hover .task-edit {
    display: inline;
}
.task .task-edit {
    float: right;
    display: none;
}
.pointer:hover {
    opacity: 0.7;
}
.fa, .fas {
    font-weight: 900;
}
.fa, .far, .fas {
    font-family: "Font Awesome 5 Free";
}
.fa, .fab, .fad, .fal, .far, .fas {
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    display: inline-block;
    font-style: normal;
    font-variant: normal;
    text-rendering: auto;
    line-height: 1;
}
.pointer {
    cursor: pointer !important;
}


.navbar .app-title {
    justify-content: space-around;
    font-family: "Comic Sans", "Comic Sans MS", cursive;
    font-size: 1.3em;
}
.navbar > * {
    width: 300px;
    display: flex;
    flex-direction: row;
    align-items: center;
}
.navbar .actions {
    justify-content: flex-end;
}
.navbar > * {
    width: 300px;
    display: flex;
    flex-direction: row;
    align-items: center;
}
.navbar .menu > *, .navbar .actions > * {
    display: inline-block;
    padding: 8px;
    border-radius: 2px;
    margin: 0px 4px;
    background-color: rgba( 64, 144, 172, 1 );
}
.board-container {
    display: flex;
    height: 100vh;
    overflow-y: hidden;
}
.board-menu {
    position: fixed;
    top: 50px;
    right: 0px;
    left: 0px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 40px;
    padding: 0 20px;
    color: black;
    background-color: rgba( 128, 128, 128, 0.3 );
    color: white;
}

html, body, div, span, applet, object, iframe, h1, h2, h3, h4, h5, h6, p, blockquote, pre, a, abbr, acronym, address, big, cite, code, del, dfn, em, img, ins, kbd, q, s, samp, small, strike, strong, sub, sup, tt, var, b, u, i, center, dl, dt, dd, ol, ul, li, fieldset, form, label, legend, table, caption, tbody, tfoot, thead, tr, th, td, article, aside, canvas, details, embed, figure, figcaption, footer, header, hgroup, menu, nav, output, ruby, section, summary, time, mark, audio, video {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;
    vertical-align: baseline;
}

.board {
    display: flex;
    flex-basis: 100%;
    flex-wrap: nowrap;
    overflow: auto;
    margin-top: 20px;
    padding: 84px 20px 20px;
}
.task-list-wrapper {
    flex-shrink: 0;
    flex-basis: 240px;
    max-height: 100%;
    overflow: hidden;
}
.task-list {
    padding: 10px;
    margin-right: 10px;
    border-radius: 4px;
    background-color: rgba( 240, 240, 240, 0.9 );
}

.task-list-title-container {
    display: flex;
    justify-content: space-between;
}
.task-list-title {
    margin: 4px;
    font-weight: bold;
}

.task-list-more {
    margin: 0 4px;
}
            .btn-primary {
    background-color: olive;
    color: white;
}

        </style>
    </head>
    <body>
        <nav class="navbar">
            <ul class="menu">
                <li class="pointer">
                    <i class="fa fa-home"></i>
                </li>
                <li class="pointer">
                    <i class="boards fas fa-th-list"></i>
                    Boards
                </li>
                <li class="menu-input">
                    <input type="text">
                </li>
            </ul>
            <div class="app-title">
                Tralala
            </div>
            <div class="actions">
                <span class="pointer">
                    <i class="fas fa-plus" id="add-board"></i>
                </span>
                <span class="pointer">
                    <i class="fas fa-user" id="profile-image"></i>
                </span>
            </div>
        </nav>
        <div class="board-menu">
            <div class="board-title">Frontend Training</div>
            <div class="board-show-menu pointer">
                <i class="fa fa-ellipsis-v"></i>
                Show menu
            </div>
        </div>
        <div class="board">
            <div class="task-list-wrapper">
                <div class="task-list">
                    <div class="task-list-title-container">
                        <h3 class="task-list-title">To Do</h3>
                        <span class="task-list-more pointer">...</span>
                    </div>
                    <div class="task pointer">
                        Learn HTML
                        <i class="task-edit fas fa-pencil-alt pointer"></i>
                    </div>
                    <div class="task pointer">
                        Learn CSS
                        <i class="task-edit fas fa-pencil-alt pointer"></i>
                    </div>
                    <div class="task pointer">
                        Learn JavaScript
                        <i class="task-edit fas fa-pencil-alt pointer"></i>
                    </div>
                    <div class="add-card-message pointer">+ Add another card</div>
                </div>
            </div>
            <div class="task-list-wrapper">
                <div class="task-list">
                    <div class="task-list-title-container">
                        <h3 class="task-list-title">Doing</h3>
                        <span class="task-list-more pointer">...</span>
                    </div>
                    <div class="task pointer">Prepare resume</div>
                    <div class="add-card-form">
                        <form>
                            <textarea rows="3" placeholder="Enter a title for this card..." class="full-width-input"></textarea>
                            <div class="add-card-form-actions">
                                <button class="btn btn-inline btn-primary add-card-button pointer">Add Card</button>
                                <i class="fas fa-2x fa-times add-card-cancel pointer"></i>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
            <div class="task-list-wrapper">
                <div class="task-list">
                    <div class="task-list-title-container">
                        <h3 class="task-list-title">Testing/Verifying</h3>
                        <span class="task-list-more pointer">...</span>
                    </div>
                    <div class="task pointer">Twitter app frontend</div>
                    <div class="add-card-message pointer">+ Add another card</div>
                </div>
            </div>
            <div class="task-list-wrapper">
                <div class="task-list">
                    <div class="task-list-title-container">
                        <h3 class="task-list-title">Deploying</h3>
                        <span class="task-list-more pointer">...</span>
                    </div>
                    <div class="task pointer">Twitter app backend</div>
                    <div class="add-card-message pointer">+ Add another card</div>
                </div>
            </div>
            <div class="task-list-wrapper">
                <div class="task-list">
                    <div class="task-list-title-container">
                        <h3 class="task-list-title">Done</h3>
                        <span class="task-list-more pointer">...</span>
                    </div>
                    <div class="add-card-message pointer">+ Add card</div>
                </div>
            </div>
            <div class="task-list-wrapper">
                <div class="task-list">
                    <div class="add-list-message pointer">+ Add another list</div>
                </div>
            </div>
            <div class="task-list-wrapper">
                <div class="task-list">
                    <div class="add-card-form">
                        <form>
                            <textarea rows="3" placeholder="Enter list title..." class="full-width-input"></textarea>
                            <div class="add-list-form-actions">
                                <button class="btn btn-inline btn-primary add-list-button pointer">Add List</button>
                                <i class="fas fa-2x fa-times add-list-cancel pointer"></i>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </body>
</html>
 
