# BoatAttack with ML-Agents (Linux Build - 1.0)

<h4 align="center">
This branch contains the Linux build version of <a href="https://github.com/Dhyeythumar/BoatAttack-with-ML-Agents">BoatAttack with ML-Agents</a> repo.
</h4>

> **Note:**
>
> -   If you want to try out the **BoatAttack with ML-Agents**, then fork and clone this repo.
> -   You will find various build versions on different branches.
> -   Now checkout the branch suitable to your OS and run the executable file. 😎

## Environment Details

![BoatAttack](https://raw.githubusercontent.com/Dhyeythumar/impression/master/boat_attack_assets/env.png)

-   Set-up: Environment where the agent needs to complete the lap in a minimum amount of time
-   Goal: Reach the finishing line in a minimum amount of time
-   Agents: The environment contains one agent (boat)
-   Agent Reward Function (independent):
    -   Speed \* 0.001 at each step
    -   -1.0 when agent crashes
    -   checkpoint value \* 0.0001
-   Behavior Parameters:
    -   Vector Observation space: 171 variables corresponding to
        -   56 ray-casts stacked 3 times to capture motion (Total 168 ray-casts) each detecting one of two possible objects (boundary & ground)
        -   1 variable stacked 3 times to capture the speed  (Total 3 variable) of the agent
    -   Vector Action space (Continuous): Size of 2 correspondings to agents rotation and forward/backward movement
    -   Visual Observations (Optional): None
-   Benchmark Mean Reward: (Yet to find)

## License

Licensed under the [MIT License](./LICENSE).

## Acknowledgements

-   [Boat Attack](https://github.com/Unity-Technologies/BoatAttack) environment by Unity Technology.
