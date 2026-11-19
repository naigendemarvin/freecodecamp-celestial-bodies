
Celestial Bodies Database

A relational PostgreSQL database modeling galaxies, stars, planets, moons, and planetary missions, built for the freeCodeCamp Relational Database Certification. The project demonstrates normalized database design using primary keys, foreign key relationships, unique constraints, and varied PostgreSQL data types.

Project Structure

• universe.sql — Complete PostgreSQL database dump containing the universe schema, table definitions, constraints, and all populated astronomical records.

Database Schema

• galaxy — Stores major galaxies (e.g., Milky Way, Andromeda, Triangulum) with descriptions, galaxy types, age, and distance from Earth.
• star — Stores stars linked to their host galaxy_id, including spectral type, temperature, mass, and spherical status.
• planet — Stores planets orbiting a specific star_id, tracking planet type, orbital characteristics, distance from star, and potential for life.
• moon — Stores natural satellites linked to their parent planet_id, including radius, orbital period, and surface notes.
• mission (or 5th custom table) — Tracks space exploration missions or astronomical observations linked to target celestial bodies.

Key Database Features

• Relational Integrity: Enforces parent-child hierarchies across galaxy → star → planet → moon using PRIMARY KEY and FOREIGN KEY constraints.
• Data Validation: Applies NOT NULL and UNIQUE constraints across key identifiers and names to prevent duplicate or incomplete records.
• Diverse Data Types: Utilizes SERIAL, INT, NUMERIC, TEXT, VARCHAR, and BOOLEAN columns tailored to astronomical measurements.


Technologies Used

• PostgreSQL
• SQL
