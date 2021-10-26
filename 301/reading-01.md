# Read: Class 01 - Component-Based Architecture & Props

## Component-Based Architecture
from 
  
  1. What is a "component"?
    - A modular set of functionality that encapsulates its implementation
    - a "building block" for a larger piece of functionality
  2. What are the characteristics of a component?
    - Reusability
    - Replaceable
    - Not context specific
    - Extensible
    - Encapsulated
    - Independent
  3. What are the advantages of using component-based architecture?
    - Ease of deployment
    - Reduced cost
    - Ease of development
    - Reusable
    - Modification of technical complexity
    - Reliability
    - System maintenance and evolution
    - Independent

## What is Props and How to Use in React
from

  1. What is "props" short for?
    - "props" is a keyword in React which is used to pass data down from one component to another
  2. How are props used in React?
    - props work very much like html attributes

    ``` js
        class Parent extends Component {
            render() {
                return (
                    <>
                        <Child text={"1"} />
                        <Child text={"2"} />
                    </>
                )
            }
        }

        class Child extends Component {
            render() {
                return (
                    <>
                        <p>{props.text}</p>
                    </>
                )
            }
        }
    ```
  3. What is the flow of props?
    - props flow downward from parent to child
