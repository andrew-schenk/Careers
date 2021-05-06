
# Technical 1
### Frontend JavaScript
If you are applying for a frontend developer position, please complete this section.

#### Task
Convert this class component into a functional component.


```javascript
import React from 'react';

class MyComponent extends React.Component(props) {

    componentDidMount() {

        this.props.fetchDrafts()
        this.props.fetchHistory()

        this.fetchDraftsTimer = setInterval(() => {
            this.props.fetchDrafts();
        }, 120000);
    }
    
    render() {
        return null;
    }

}
```

Create a gist to hold your answer.  Email the gist link to careers@linxsystems.com


**Do not post your answer here.**
