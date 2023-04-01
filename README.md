```yaml
import React from 'react';

class About extends Me {
  getCurrentWorkplace() {
    return {
      workplace: {
        company: 'IKY GROUP',
        position: 'Web Developer'
      }
    };
  }

  getDailyKnowledge() {
    return [
      'React',
      'Bootstrap',
      'Sass',
      'Redux',
      'TailwindCss',
      'Javascript',
      'Nodejs'
    ];
  }

  getFutureGoal() {
    return 'To contribute to open source.';
  }

  render() {
    return (
      <div>
        <h1>About Me</h1>
        <p>Current Workplace: {this.getCurrentWorkplace().workplace.company} - {this.getCurrentWorkplace().workplace.position}</p>
        <p>Daily Knowledge: {this.getDailyKnowledge().join(', ')}</p>
        <p>Future Goal: {this.getFutureGoal()}</p>
      </div>
    );
  }
}

export default About;
```
