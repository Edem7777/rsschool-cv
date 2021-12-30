# Abibullaev Edem Rustemovich
### My phone and email: _+7 978 004 10 75_, _edemabibullaev95@mail.ru_
### Short summary about me: _My goal is to develop in the field of programming. The motivation is a high salary and the opportuniti to work in a team._
### Skills: _blind printing, teamwork, JS-developer_
### My code: 
```
const board = document.querySelector('#board')
const colors = ['red', 'blue', 'orange', 'green', '#de1212', '#484f5c', '#042259', '#ffffff', '#cc11d6', '#c4ff00']
const RELIZ_NUMBER = 1276

for(let i = 0; i < RELIZ_NUMBER; i++) 
    {
        const reliz = document.createElement('div')
        reliz.classList.add('reliz')

            reliz.addEventListener('mouseover', () =>
                setColor (reliz))
            
            reliz.addEventListener('mouseleave', () => 
                removeColor (reliz))

        board.append(reliz)
    }

function setColor (element) {
    const color = getRandomColor()
    element.style.backgroundColor = color
    element.style.boxShadow = `0 0 2px ${color}, 0 0 15px ${color}`
}

function removeColor (element) {
    element.style.backgroundColor = 'rgb(24, 39, 8)'
    element.style.boxShadow = `0 0 2px rgb(24, 39, 8)`
}

function getRandomColor() {
    const index = Math.floor(Math.random() * colors.length)
    return colors[index]
}
```
### Education: _communications engineer_
### English level: _Intermediate_