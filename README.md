# prettier-kanban4calm @sabatale
## _A prettier version of SAP Cloud ALM Kanban_

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

This is a fork from [the official SAP CALM Sample repo](https://github.com/SAP-samples/cloud-alm-api-examples/tree/main/applications/kanban4calm).
I wanted to show off what an actual Kanban board may look like with a modern theme, and some additional features.
This is by no means productive-ready or bug-free, but this sample should give you a head start.

[Check the demo here.](https://github.com/sabatale/prettier-kanban4calm/blob/main/demo.mp4)

## Important

Because the tasks details are also fetched (e.g. description), it is NOT recommended to display all standard Template Tasks. If you do, the details are fetched asynchronously so you may have to wait a few seconds before being able to display those for all your tasks.

## Features

- Select your SAP CALM Project
- Load the project tasks (type, title, due date, priority)
- Display the tasks details (id, phase, description, assignee)
- Drag & Drop tasks in the Kanban lanes to update status
- Rename tasks on the fly
- Filter (default ON) to hide Template tasks
- Loading icon whenever the API is loading data
- Status notifications for API requests

## Tech

This sample is making some changes compared to the original:

- Implement a new theme (forked [@AaronMcGuire](https://codepen.io/aaronmcg/pen/GRjaRva))
- Replace SortableJS with [Dragula](https://github.com/bevacqua/dragula)
- Make use of [Bootstrap Modals](https://getbootstrap.com/docs/4.6/components/modal/) for the tasks edit
- Add [Bootstrap-Switch](https://github.com/Bttstrp/bootstrap-switch) for the filter toggle
- Add [Toastify-js](https://github.com/apvarun/toastify-js) for notifications

And of course the sample itself is open source.

## Installation

prettier-kanban4calm requires [Node.js](https://nodejs.org/) v12+ to run.

Rename the file config.json.sample and add your API information.

Install the dependencies and devDependencies and start the server.

```sh
npm install
npm run dev
```

The server should now run on port 3000.

## License

Apache License 2.0
