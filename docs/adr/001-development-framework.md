# 001: Development Framework (React Native)

## Status
Accepted

## Context
we need to select a cross-platform framework that would support the development of a clean, simple Android music player efficiently, minimizing development time and aligning with the team's skillset.

## Decision
The application will be built using **React Native**.

## Rationale
React Native allows us to use a single JavaScript/TypeScript codebase for our target platform, which significantly accelerates development. It also provides the essential access to native device features (speaker, storage) that a music player requires. This decision maintains the stability established in Phase 1 and reduces overall project risk.

## Consequences
The team is fully committed to the React Native ecosystem, requiring adherence to its specific component libraries and build processes for the entire duration of the project.
