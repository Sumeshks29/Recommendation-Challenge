# Recommendation-Challenge
Improve the user experience on a fast-growing mobile platform,
for hosting coding challenges

Your client is a fast-growing mobile platform, for hosting coding challenges. They have a unique business
model, where they crowdsource problems from various creators(authors). These authors create the
problem and release it on the client's platform. The users then select the challenges they want to solve.
The authors make money based on the level of difficulty of their problems and how many users take up
their challenge.
The client, on the other hand makes money when the users can find challenges of their interest and
continue to stay on the platform. Till date, the client has relied on its domain expertise, user interface and
experience with user behaviour to suggest the problems a user might be interested in. You have now
been appointed as the data scientist who needs to come up with the algorithm to keep the users engaged
on the platform.
The client has provided you with history of last 10 challenges the user has solved, and you need to
predict which might be the next 3 challenges the user might be interested to solve. Apply your data
science skills to help the client make a big mark in their user engagements/revenue.

Dataset description:
We have three data files,
- Train.csv
1. user_sequence - Unique ID for the sequence
2. user_id - User ID
3. challenge _sequence - Challenge sequence number(1-13)
4. challenge - Challenge ID

- Challenge.csv
1.Challenge_ID - Challenge_ID
2.programming _language - Programming language for the challenge
3.challenge_series _ID - Series for the given challenge
4.total_submissions - Total submission by all users
5.publish_date - Publishing date for the challenge
6.author_ID - Author ID
7.author_org_ID - Organization ID for author
8.category_id - Type of challenge

Evaluation Metric
- The evaluation metric is Mean Average Precision (MAP) at K (K = 3). MAP is a well-known metric
used to evaluate ranked retrieval results. E.g. Let’s say for a given user, we recommended 3
challenges and only 1
st and 3
rd challenges are correct. So, the result would look like — 1, 0, 1
- In this case, The precision at 1 will be: 11/1 = 1 The precision at 2 will be: 01/2 The precision at 3
will be: 1*2/3 = 0.67 Average Precision will be: (1 + 0 + 0.67)/3 = 0.556.
