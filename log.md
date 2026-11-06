# Log

## Day 1 (Oct 15)
- Set up the repo
server replies with sataus code 200=ok   201 = created  302= redirect
react basics 

to create new appln = npm create vite@latest
then cd part1 then npm install
The App.jsx file now defines a React component called App . The last line of the main.jsx file defines the command
react components r written using jsx then the jsx returned by eact components is translated to js
JSX is "XML-like", meaning that each tag must be closed  <br/>
A component is any function with a capital letter that returns JSX. 
a cmponent returns one root e/t like<div>
to add to the github => git status => git add .then git commit -m"exercise 1.1 and 1.2 then git push
part 1b
const and let const canht be reassigned and let can but if cons is an array we can change it using the term t.push
never use var
array
t.foreach(value =>{
    console.log
}) it runs throgh the list and runs ur fucnction once per item
t.map(value => value*2) craets a new row which is twicw thw amount os the first row
## Day 2 (oct 30)
React works best with data that isn't changed in place. concat gives you a new array, while push changes the old one.
## part 1c
*helper fun insde a component
new Date().getFullYear() means “get today’s year
you write Hello and bornYear, and JavaScript gives you Date and getFullYear
*instead of using props again and again we can do
const Hello = ({ name, age }) => {
  // now use name and age directly, no "props." needed
} its the same
an event handler is a function
<button onclick {()=> setCounter(counter+1)}>plus</button>
## part 1d
const [left, setLeft] = useState(0) when we write smthng like thisreact dont change when we increse or decrese a number so we do <button onClick={() => setLeft(left + 1)}>left</button> to increse the number that  in the left and the changed result is saved in diffrent box
setAll(allClicks.concat('L')) this means make a new longer strip that has everything from the old one and plus an l at the end . and its wrong to use push
Use a separate useState for each separate thing.
Never change state directly. Always use the setter (the robot).
Give the robot a new object or a new list: { ...old, field: newValue } for objects, old.concat(item) for lists.
join is only for showing a list as text.
Anything inside <div>...</div> is shown on the page as text. Calculations are JavaScript, so they go above the return, before any JSX