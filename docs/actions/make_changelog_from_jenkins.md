<!--
This file is auto-generated and will be re-generated every time the docs are updated.
To modify it, go to its source at https://github.com/fastlane/fastlane/blob/master/fastlane/lib/fastlane/actions/make_changelog_from_jenkins.rb
-->

# make_changelog_from_jenkins


Generate a changelog using the Changes section from the current Jenkins build




> This is useful when deploying automated builds. The changelog from Jenkins lists all the commit messages since the last build.


make_changelog_from_jenkins ||
---|---
Supported platforms | ios, android, mac
Author | @mandrizzle



## 1 Example

```ruby
make_changelog_from_jenkins(
  # Optional, lets you set a changelog in the case is not generated on Jenkins or if ran outside of Jenkins
  fallback_changelog: "Bug fixes and performance enhancements"
)
```





## Parameters

Key | Description | Default
----|-------------|--------
  `fallback_changelog` | Fallback changelog if there is not one on Jenkins, or it couldn't be read | `''`
  `include_commit_body` | Include the commit body along with the summary | `true`

<em id="parameters-legend-dynamic">* = default value is dependent on the user's system</em>


<hr />

## Documentation

To show the documentation in your terminal, run
```no-highlight
fastlane action make_changelog_from_jenkins
```

<hr />

## CLI

It is recommended to add the above action into your `Fastfile`, however sometimes you might want to run one-offs. To do so, you can run the following command from your terminal

```no-highlight
fastlane run make_changelog_from_jenkins
```

To pass parameters, make use of the `:` symbol, for example

```no-highlight
fastlane run make_changelog_from_jenkins parameter1:"value1" parameter2:"value2"
```

It's important to note that the CLI supports primitive types like integers, floats, booleans, and strings. Arrays can be passed as a comma delimited string (e.g. `param:"1,2,3"`). Hashes are not currently supported.

It is recommended to add all _fastlane_ actions you use to your `Fastfile`.

<hr />

## Source code

This action, just like the rest of _fastlane_, is fully open source, <a href="https://github.com/fastlane/fastlane/blob/master/fastlane/lib/fastlane/actions/make_changelog_from_jenkins.rb" target="_blank">view the source code on GitHub</a>

<hr />

<a href="/actions/"><b>Back to actions</b></a>
