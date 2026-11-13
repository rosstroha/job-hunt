# Job Hunt

This is a repository to store metadata on job postings from various sources.

The user is looking for a software job at Senior or higher. Their current level is Software Engineer III.

Do not save a job if it already exists. Base this off its source's unique identifier.

## Job Metadata

1. Unique identifier from the source website
2. Title
3. Status
  1. Retrieved (meaning pulled from the source and its information is here in this repo).
  2. Viewed
  3. Ignored - It's a no-go for any reason.
  4. Matched - Agent determine match for me based on the job metadata  and README.md.
  5. Interested - The user may apply to this position.
  4. Applied
  5. Employer declined - turned down by the company after applying.
4. Company name
5. Stated salary, if any. Leave blank if there is none. Colorado is the state that matters.
6. URL
7. Remote, in-person, hybrid (location)
8. Description
9. Brief, one-sentence match rationale, if there is a match, otherwise skip this sentence. Follow this by a brief one sentence on why it doesn't match because not all matches will be 100% a match. If the job is a perfect fit, then don't add a second sentence.

## Sources

1. Linkedin - Metadata retrieval is done using the guidance from /home/ross/Projects/linkedin-job-export

## Job Matching Criteria

1. If the agent has not read README.md already, do it now.
2. The stated salary is no more than $10k under the user's current salary, which is never to be committed to git. It's to be stored in memory and this is where the agent should check first if it does not already know.
3. Remote is highly prefered over hybrid or in-person only. When the job aligns with personal interests, the user will consider non-remote positions and they should be considered a potential match (Job metadata #3.4).
4. The position requires align with past experience. The user's resume will be added to this repo root.
5. It is a software engineering or development position.
6. The salary is only considered for matching when it is stated in the listing.
7. Positions higher than Senior should be more carefully considered for qualification.

## Personal Interests

### Definite yesses (with no specific priority)

1. RV, vanlife, DIY van building.
2. IoT relating to home automation, Home Assistant, Esphome, zigbee, zwave, etc.
3. Video games or companies that relate to them.
4. Woodworking
5. Pets/Animal care
6. 3D printing
7. Drones/RC
8. Bicycling
9. Outdoor recreation
10. Snowboarding

### Definite No's

1. Companies the user has worked at already.
2. IBM, Amazon, Google, Meta (or subsidary companies), Netflix

### Everything else

Weigh these neutrally.

## Job posting storage format

Keep separate per-job json files in the following structure: `jobs` -> `source` -> `company`. The filename should be the trucated position title and id.

