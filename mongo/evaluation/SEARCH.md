# In order to locate texts in documents in mongodb, it`s no use using find() method with a text param like this:
# db.movies.find({ movie: "musical" }) cause this method look for exact match for fetching data, stead use alternatives ways to do that.

# regex, expr