This project given Below is a backend implementaion of Todo App as asked by the problem.
The code is based on MVC(Model View Controller) architecture with default routes as -

createTodo-(PUT)http://localhost:3000/api/v1/createTodo
getTodos-(GET)http://localhost:3000/api/v1/getTodos
getTodo/:id-(GET)http://localhost:3000/api/v1/getTodos/:id
updateTodo/:id-(PUT)http://localhost:3000/api/v1/updateTodo/:id
deleteTodo/:id-(DELETE)http://localhost:3000/api/v1/deleteTodo/:id

The Database used is mongoDB and delfault shema is -
        title:{
            type:String,
            required:true,
            maxLength:50,
        },
        description: {
            type:String,
            required:true,
            maxLength:50,
        },
        createdAt:{
            type:Date,
            required:true,
            default:Date.now(),
        },
        updatedAt:{
            type:Date,
            required:true,
            default:Date.now(),
        }

Initilization of project includes-
1. npm init -y
2. npm i express nodemon dotenv mongoose
3. To start the server use command - npm run dev
