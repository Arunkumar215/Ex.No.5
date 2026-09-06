# Ex.No.5 – Comparing Prompting Techniques Through Engineering Problem-Solving Scenarios


## Reg. No.:
212223220009

## Aim

To compare different prompting techniques and evaluate their effectiveness in solving a real-world engineering problem from the student's project by analyzing the relevance, accuracy, completeness, clarity, feasibility, and usefulness of AI-generated solutions.

## AI Tools Required

- ChatGPT
- Google Gemini
- Microsoft Copilot

# Experiment Overview

In this experiment, a genuine problem from the **Sports Club Management System** project is selected. The same engineering problem is given to an AI system using different prompting techniques.

The generated responses are compared to understand how changes in prompt structure affect the quality, accuracy, depth, and usefulness of the solution.

## Project Title

**Sports Club Management System**

## Problem Statement

The Sports Club Management System is designed to manage sports club activities including members, coaches, sports activities, events, schedules, facilities, and payments.

A major problem is efficiently managing member schedules and avoiding conflicts between coaches, sports activities, facilities, and events. Manual scheduling can result in overlapping bookings, unavailable facilities, and conflicts between members and coaches.

The objective is to develop an effective scheduling approach that can identify conflicts and recommend suitable schedules.

# Step 1 – Select the Engineering Problem

### Selected Engineering Scenario

**Conflict-Free Sports Club Scheduling**

### Engineering Problem

Design a scheduling method for a Sports Club Management System that manages members, coaches, sports activities, events, and facilities while preventing schedule conflicts.

The system should identify overlapping schedules and suggest suitable available time slots.

# Step 2 – Base Prompt

A simple prompt was created without using advanced prompting techniques.

### Base Prompt

> Design a scheduling system for a Sports Club Management System that avoids conflicts between members, coaches, sports activities, and facilities.

### AI-Generated Response

The system can use a centralized scheduling module to store information about members, coaches, activities, facilities, and available time slots.

Before creating a schedule, the system can check whether the selected coach, member, or facility is already assigned to another activity during the same time period.

If a conflict is detected, the system can suggest another available time slot. The schedule can be stored in a database and displayed to users through the application.

# Step 3 – Apply Different Prompting Techniques

The same engineering problem was rewritten using different prompting techniques.

## Technique 1 – Straightforward Prompt

### Prompt

> Suggest a method to detect and prevent scheduling conflicts between members, coaches, sports activities, and facilities in a Sports Club Management System.

### Output

A scheduling module can maintain the availability of members, coaches, and facilities. Before assigning an activity, the system checks for overlapping time slots. If an overlap exists, the system rejects the booking and suggests another available slot.

### Observation

The response provides a basic solution but does not explain the implementation in detail.

---

# Technique 2 – Query Decomposition

Query decomposition breaks a complex engineering problem into smaller and manageable tasks.

### Prompt

> Solve the scheduling problem in a Sports Club Management System by breaking it into the following tasks:
>
> 1. Identify scheduling requirements.
> 2. Identify the resources involved.
> 3. Detect scheduling conflicts.
> 4. Check resource availability.
> 5. Suggest alternative time slots.
> 6. Explain how the solution can be implemented in a software system.
>
> Provide a clear and structured solution for each task.

### Output

### 1. Scheduling Requirements

The system should manage activities, members, coaches, facilities, dates, and time slots.

### 2. Resources

The main resources are:

- Members
- Coaches
- Sports activities
- Facilities
- Events
- Time slots

### 3. Conflict Detection

The system should compare the requested time slot with existing schedules.

A conflict occurs when the same member, coach, or facility is already assigned during the requested period.

### 4. Availability Checking

The system checks the availability of all required resources before confirming a booking.

### 5. Alternative Time Slots

If a conflict occurs, the system searches for available time slots and recommends suitable alternatives.

### 6. Implementation

The scheduling information can be stored in a database. A scheduling algorithm can check existing records before creating a new booking.

### Observation

Query decomposition produced a more complete and logically organized solution.

---

# Technique 3 – Role-Based Prompting

Role-based prompting assigns a specific role to the AI model.

### Prompt

> Act as a software architect designing a Sports Club Management System. Design a reliable scheduling module that prevents conflicts between members, coaches, sports activities, events, and facilities.
>
> Explain:
>
> - System requirements
> - Conflict detection method
> - Scheduling logic
> - Database requirements
> - Alternative slot recommendation
> - Error handling
>
> Provide a practical solution suitable for a college engineering project.

### Output

The scheduling module should use a centralized schedule database containing activity ID, member ID, coach ID, facility ID, date, start time, and end time.

When a user requests a new booking, the system should verify all required resources.

The system should check:

- Member availability
- Coach availability
- Facility availability
- Time-slot availability

If any resource has an overlapping booking, the request should be rejected or an alternative time should be suggested.

### Observation

The role-based prompt generated a more technical and implementation-oriented response.

---

# Technique 4 – Constraint-Based Prompting

Constraint-based prompting provides specific conditions that the AI solution must satisfy.

### Prompt

> Design a scheduling solution for a Sports Club Management System using the following constraints:
>
> - A coach cannot manage two activities at the same time.
> - A facility cannot be assigned to two activities at the same time.
> - A member cannot register for two activities at the same time.
> - Every activity must have an assigned coach.
> - Every activity must have an available facility.
> - The system should detect conflicts before confirming a booking.
> - If a conflict occurs, suggest at least two alternative available time slots.
> - Explain the solution using simple technical language.

### Output

The scheduling system should validate every booking against the defined constraints.

For a requested activity, the system checks whether the selected coach, facility, and members are already assigned during the requested time.

If no conflict is found, the booking is confirmed.

If a conflict is detected, the system identifies available time slots and provides alternative options.

### Observation

The constraint-based prompt produced the most specific solution because the required conditions were clearly defined.

---

# Step 4 – Comparison of Prompting Techniques

| Prompting Technique | Relevance | Accuracy | Completeness | Clarity | Feasibility |
|---|---|---|---|---|---|
| Straightforward Prompt | Good | Good | Moderate | Good | Good |
| Query Decomposition | Very Good | Good | Very Good | Very Good | Very Good |
| Role-Based Prompting | Very Good | Very Good | Very Good | Very Good | Very Good |
| Constraint-Based Prompting | Excellent | Very Good | Excellent | Very Good | Excellent |

# Step 5 – Analysis and Observations

The responses generated using different prompts were analyzed based on their quality and usefulness.

### Observations

1. The straightforward prompt produced a general solution.
2. Query decomposition improved the structure and completeness of the response.
3. Role-based prompting produced a more professional software architecture perspective.
4. Constraint-based prompting produced the most specific solution because the system requirements were clearly defined.
5. Providing detailed constraints reduced ambiguity.
6. Advanced prompts produced more useful engineering solutions than simple prompts.
7. Human review is still required to verify the technical feasibility of the solution.

# Naïve Prompt vs Improved Prompt

| Factor | Naïve / Basic Prompt | Improved Prompt |
|---|---|---|
| Problem description | General | Detailed |
| Context | Limited | Project-specific |
| Constraints | Not specified | Clearly defined |
| Output structure | General response | Structured solution |
| Technical depth | Moderate | High |
| Accuracy | Moderate | Better |
| Completeness | Limited | High |
| Practical usefulness | Moderate | High |

# Step 6 – Final Selected Prompting Technique

Based on the comparison, **Constraint-Based Prompting** was selected as the most effective technique for this engineering problem.

The technique clearly defines the conditions that the scheduling system must satisfy and helps the AI generate a solution that is more practical and specific.

# Refined / Final Prompt

> Act as a software architect and design a conflict-free scheduling module for a Sports Club Management System.
>
> The system manages members, coaches, sports activities, events, facilities, and payments.
>
> The scheduling module must satisfy the following constraints:
>
> 1. A coach cannot manage two activities at the same time.
> 2. A facility cannot be assigned to two activities at the same time.
> 3. A member cannot participate in two activities at the same time.
> 4. Every activity must have an assigned coach.
> 5. Every activity must have an available facility.
> 6. The system must check for conflicts before confirming a booking.
> 7. If a conflict occurs, the system must suggest at least two available alternative time slots.
> 8. Explain the database information required.
> 9. Explain the conflict detection logic.
> 10. Provide a practical solution suitable for implementation in a college-level software project.
>
> Present the solution using clear headings, steps, and a simple example.

# Engineering Validation

The final AI-generated solution was evaluated against the actual requirements of the Sports Club Management System.

| Validation Criteria | Status |
|---|---|
| Member conflict detection | Satisfied |
| Coach conflict detection | Satisfied |
| Facility conflict detection | Satisfied |
| Activity scheduling | Satisfied |
| Alternative slot recommendation | Satisfied |
| Database requirements | Satisfied |
| Practical implementation | Satisfied |
| Clear explanation | Satisfied |

# Key Findings

- Prompt clarity directly affects AI output quality.
- Providing project context improves relevance.
- Breaking complex problems into smaller tasks improves completeness.
- Role-based prompts improve technical depth.
- Clearly defined constraints improve feasibility.
- Iterative prompting helps produce better final solutions.
- AI-generated solutions should be validated before implementation.

# Deliverables

1. Project title and problem statement.
2. Selected engineering scenario.
3. Base prompt.
4. Minimum four improved prompts using different techniques.
5. AI-generated outputs.
6. Comparison and evaluation table.
7. Analysis and observations.
8. Final selected prompting technique.
9. Refined/final prompt.
10. Engineering validation.

# Result

The prompt comparison experiment was successfully performed using the **Sports Club Management System** scheduling problem. Different prompting techniques were applied and their outputs were compared based on relevance, accuracy, completeness, clarity, and feasibility. The constraint-based prompting technique produced the most specific and practically useful solution.

# Conclusion

Thus, the experiment successfully demonstrated that different prompting techniques can significantly affect the quality of AI-generated engineering solutions. Simple prompts provide general answers, while query decomposition, role-based prompting, and constraint-based prompting produce more structured, detailed, and practical solutions. Among the techniques tested, constraint-based prompting was found to be highly effective for solving the scheduling problem in the Sports Club Management System.
