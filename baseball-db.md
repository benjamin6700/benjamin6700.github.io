---
layout: single
title: "Baseball League Database"
permalink: /portfolio/baseball-db/
---

My Baseball League Database is a solo academic project built to design and implement a relational database in MySQL for managing a baseball league. The database tracks player and team statistics, standings, and game scheduling, giving a structured, queryable system for information that would otherwise be scattered across spreadsheets or manual records.

## My Role

As a solo project, I was responsible for the full process end to end — designing the database schema, defining relationships between entities like players, teams, and games, and writing the queries needed to support statistics tracking, standings calculations, and schedule management. Working without a team meant every design decision, from normalization choices to how stats would be aggregated, was mine to make and defend.

## Design Process

I started by mapping out the core entities the league needed to track — players, teams, games, and the stats tied to each — and worked through how they related to one another before writing any SQL. Getting the schema right up front mattered. A baseball league has layered relationships (players belong to teams, teams play games, games generate stats tied to both players and teams), so a poorly normalized structure early on would have made the stats and standings queries far messier later. Once the schema was solid, I built out the queries needed to calculate standings and pull player/team statistics on demand.

## Challenges

Working solo meant there was no one to catch design mistakes early or split up the workload. Every schema decision, query, and edge case was something I had to reason through myself. Structuring the database to handle standings and statistics cleanly took some iteration, since those numbers depend on aggregating data across multiple related tables rather than living in one place.

## Takeaways

This project gave me hands-on, ground-up experience with relational database design. This is something that's easy to gloss over in coursework that hands you a schema to work with. Building it solo also meant developing a stronger sense of ownership over the whole process, from initial design through to a working, queryable system.
