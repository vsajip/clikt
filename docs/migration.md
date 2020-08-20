# Upgrading to Newer Releases

## Upgrading to 3.0

### Environment variable splitting

There used to be an `envvarSplit` parameter to `option()` and its `convert()` that would split
values coming from an environment variable. This parameter is removed, and values from environment
variables are no longer split automatically.

If you still want to split option values, you can do so explicitly with [`split()`][split].

### Experimental APIs

The Value Source API and Completion Generation APIs no longer require opt-in. You can use these APIs
without needing the `ExperimentalValueSourceApi` or `ExperimentalCompletionCandidates` annotations.

[split][api/clikt/com.github.ajalt.clikt.parameters.options/split.md]