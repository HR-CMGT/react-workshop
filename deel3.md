# React Workshop deel 3

## CSS 

Gebruik `className` in plaats van `class` om een element een specifieke css class mee te geven.

```javascript
render() {
  return <div className="ideas">Ideas</div>
}
```
In CSS kan je deze class name gebruiken om alles dat in het component staat een style te geven:

```css
.ideas {
    margin:10px;
    background-color:#ccc;
}

.ideas h1 {
    font-size:2em;
}

.ideas p {
    font-size:1.2em;
}
```

### CSS class met IF 

Soms wil je een bepaalde CSS class alleen toepassen als een voorwaarde true is. 
```javascript
render() {
    let className = 'menu'
    if (this.state.awesome) {
        className += ' awesome'
    }
    return <span className={className}>Menu</span>
}
```

## CSS in het component

In dit voorbeeld schrijven we de CSS in het component bestand, zodat je styles en je code bij elkaar staan. Let op dat je CSS properties nu als camelCase moet schrijven. `font-size` wordt `fontSize`.


*IDEAS.JS*
```javascript
const buttonStyle = {
    padding: "10px",
    fontSize:"1.2em"
}

class Ideas extends React.Component {
    constructor() {
        super()
    }

    render() {
        return (
            <div>
                <button style={buttonStyle}>Styled button</button>
            </div>
        );
    }
}
```
# Finished workshop files

De finished files kan je vinden in de "finished" branch van deze repository.

# Meer React concepten

Je weet nu genoeg om zelf verder te kunnen leren op de [React Tutorial Site](https://reactjs.org/docs/hello-world.html). Lees de 12 pagina's onder "Main Concepts".

1. Hello World
2. Introducing JSX
3. Rendering Elements
4. Components and Props
5. State and Lifecycle
6. Handling Events
7. Conditional Rendering
8. Lists and Keys
9. Forms
10. Lifting State Up
11. Composition vs Inheritance
12. Thinking In React

# Vervolg workshop

 - [Deel 4](./deel4.md) - Een React app compileren