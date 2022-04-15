# Ideas on how to refactor this model


## Usage

```python
> health_agent_sim = HealthAgentSimulation()
health_agent_sim.run()
```

## Program

```python

class HealthAgentSimulation():
    def __init__(
        grid_size=3, 
        num_symptom_types=3, 
        age_range=30, 
        health_load_levels=3, 
        A=None, B=None, C=None, D=None
    ):
        ...define core structure using args...
           --> A, B, C, D
        
        self.agent = pymdp.Agent(A=A, B=B, C=C, D=D)
        self.env = ...
    
    def run(self):
        ...

```