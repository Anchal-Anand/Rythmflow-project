# 004: Database Storage (Hybrid: Firestore & AsyncStorage)

## Status
Accepted

## Context
A solution is needed to store valuable user-created data (playlists) reliably in the cloud while maintaining high application speed for temporary state data (playback position).

## Decision
A hybrid model will be used: **Firebase Firestore** (Remote) for persistent, critical data, and **AsyncStorage** (Local, Unencrypted) for fast caching and state data.

## Rationale
Firestore provides reliable backup and synchronization for valuable data like playlists and settings. AsyncStorage provides instant access for less critical data like current playback state. This hybrid approach optimizes for both data reliability and application performance. Access to the music files themselves remains unencrypted to ensure seamless playback.

## Consequences
The team must develop robust logic to manage synchronization and state flow between the remote Firebase database and the local application cache to prevent data conflicts and ensure data integrity.
