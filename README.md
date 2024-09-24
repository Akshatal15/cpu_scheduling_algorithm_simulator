 <h1>CPU Scheduling Algorithm Simulation</h1>

  <h2>Overview</h2>
    <p>
        This project is a web-based simulation tool that demonstrates several CPU scheduling algorithms: 
        <strong>First-Come, First-Served (FCFS)</strong>, <strong>Round Robin (RR)</strong>, 
        <strong>Shortest Job First (SJF)</strong>, and <strong>Priority Scheduling</strong>. It allows 
        users to input processes, their burst times, and other properties (like priority) to visualize 
        how different scheduling algorithms handle process execution.
    </p>
    <p>
        The simulation helps users understand the differences in how each algorithm works by showing a 
        step-by-step graphical representation of process scheduling.
    </p>

   <h2>Features</h2>
    <ul>
        <li>
            <strong>User Input:</strong>
            <ul>
                <li>Enter process names and their corresponding burst times.</li>
                <li>For Priority Scheduling, enter the priority of each process.</li>
                <li>For Round Robin, specify the time quantum.</li>
            </ul>
        </li>
        <li>
            <strong>Algorithms Supported:</strong>
            <ul>
                <li><strong>FCFS (First-Come, First-Served):</strong> Processes are executed in the order they arrive.</li>
                <li><strong>Round Robin (RR):</strong> Processes are executed cyclically, with each receiving a fixed time slice (quantum).</li>
                <li><strong>Shortest Job First (SJF):</strong> The process with the shortest burst time is executed first.</li>
                <li><strong>Priority Scheduling:</strong> Processes with higher priority are executed first. If two processes have the same priority, they are scheduled based on their arrival order.</li>
            </ul>
        </li>
        <li>
            <strong>Real-time Visual Simulation:</strong> 
            Each process is represented as a colored block on a timeline. The timeline dynamically updates to 
            show the start and end times of each process as they are executed. Processes are drawn sequentially 
            for FCFS and SJF, while Round Robin and Priority Scheduling reflect preemptive/non-preemptive behaviors 
            based on the algorithm.
        </li>
        <li>
            <strong>Dynamic Queue Management:</strong> 
            For Round Robin, if a process's burst time exceeds the quantum, it is paused and re-added to the 
            queue for the next cycle. For Priority Scheduling, processes are sorted and executed based on their 
            priority level.
        </li>
    </ul>

  <h2>Technology Stack</h2>
    <ul>
        <li><strong>HTML5:</strong> Structure of the web interface.</li>
        <li><strong>CSS3:</strong> Styling for layout and visual design.</li>
        <li><strong>JavaScript:</strong> Logic for process scheduling and real-time canvas drawing.</li>
        <li><strong>Canvas API:</strong> Used to graphically display process execution as blocks on a timeline.</li>
    </ul>

  <h2>Usage</h2>
    <ol>
        <li>Clone or download the repository.</li>
        <li>Open <code>index.html</code> in a web browser.</li>
        <li>Enter the process names, burst times, and for Priority Scheduling, process priorities.</li>
        <li>Select the scheduling algorithm you want to simulate from the dropdown menu.</li>
        <li>For Round Robin, specify the time quantum.</li>
        <li>Click the "Start Simulation" button to visualize the process execution.</li>
    </ol>

  <h3>Example</h3>
    <ul>
        <li><strong>FCFS Input:</strong> 
            <ul>
                <li>Processes: P1, P2, P3</li>
                <li>Burst Times: 24, 3, 3</li>
            </ul>
        </li>
        <li><strong>Round Robin Input:</strong> 
            <ul>
                <li>Processes: P1, P2, P3</li>
                <li>Burst Times: 24, 3, 3</li>
                <li>Quantum: 4</li>
            </ul>
        </li>
        <li><strong>SJF Input:</strong> 
            <ul>
                <li>Processes: P1, P2, P3</li>
                <li>Burst Times: 6, 2, 8</li>
            </ul>
        </li>
        <li><strong>Priority Scheduling Input:</strong> 
            <ul>
                <li>Processes: P1, P2, P3</li>
                <li>Burst Times: 6, 2, 8</li>
                <li>Priorities: 1, 3, 2</li>
            </ul>
        </li>
    </ul>

   <h2>Algorithm Overview</h2>
    <ul>
        <li><strong>First-Come, First-Served (FCFS):</strong> 
            The process that arrives first is executed first. No preemption—once a process starts, it runs to completion.
        </li>
        <li><strong>Round Robin (RR):</strong> 
            Each process is assigned a fixed time quantum. If a process doesn’t complete in its time slice, it is paused and requeued until its next turn.
        </li>
        <li><strong>Shortest Job First (SJF):</strong> 
            The process with the shortest burst time is executed first. Preemptive and non-preemptive versions can be implemented based on the logic.
        </li>
        <li><strong>Priority Scheduling:</strong> 
            Each process is assigned a priority level. The process with the highest priority (lowest number) is executed first. If two processes have the same priority, they are executed in the order of arrival.
        </li>
    </ul>

   <h2>Future Enhancements</h2>
    <ul>
        <li>Adding support for <strong>Preemptive SJF</strong> to simulate more real-world conditions where short processes can interrupt longer ones.</li>
        <li>Displaying performance metrics such as average waiting time, turnaround time, and CPU utilization for each algorithm.</li>
        <li>Including more interactive features like draggable processes or custom animations for process switching.</li>
    </ul>

   <h2>Contribution</h2>
    <p>Contributions are welcome! Feel free to fork this repository, submit issues, or create pull requests with suggestions or improvements.</p>

    


