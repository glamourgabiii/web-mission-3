# Mission 3

## Part 0

[Link to video](https://drive.google.com/file/d/15G0ONgP7RZJ_C8p_kwxGJC4ye0zNGwf4/view?usp=sharing)

## Part1

`SELECT username
FROM users;`

`SELECT u.username, COUNT(m.id) AS sent_messages
FROM messages m
JOIN users u ON u.id = m."from"
GROUP BY u.username;`

`SELECT u.username, COUNT(m.id) AS received_messages
FROM messages m
JOIN users u ON u.id = m."to"
GROUP BY u.username
ORDER BY received_messages DESC
LIMIT 1;`

`SELECT AVG(sent_count) AS avg_sent_messages
FROM (
    SELECT u.id, COUNT(m.id) AS sent_count
    FROM users u
    LEFT JOIN messages m ON u.id = m."from"
    GROUP BY u.id
) AS user_sent_counts;`
