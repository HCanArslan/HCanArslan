```yaml
import React from 'react';

class About extends Me {
  getCurrentWorkplace() {
    return {
      workplace: {
        company: 'Hogarth',
        position: 'Frontend Developer'
      }
    };
  }

  getDailyKnowledge() {
    return [
      'React',
      'Nextjs',
      'Redux',
      'Tailwind',
      'Javascript',
      'Nodejs'
    ];
  }

  getFutureGoal() {
    return '?';
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
