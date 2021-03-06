# gc_score

The API endpoint to fetch the activities for a user on Github is as follows:

[https://api.github.com/users/username/events/public](https://api.github.com/users/username/events/public)

The JSON response for the above call contains an area of events of different types, and
each event has a score attached to it.

The following mapping shows the scores available:

```ruby
{
"IssuesEvent" => 7,
"IssueCommentEvent" => 6,
"PushEvent" => 5,
"PullRequestReviewCommentEvent" => 4,
"WatchEvent" => 3,
"CreateEvent" => 2
}
```

**Write a program in Ruby which would fetch the commit score for a user on Github.**
