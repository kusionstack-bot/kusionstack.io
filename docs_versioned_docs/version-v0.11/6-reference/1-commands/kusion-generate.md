## kusion generate

Generate versioned Spec of target Stack

### Synopsis


		Generate versioned Spec of target Stack. 
	
		The command must be executed in a Stack or by specifying a Stack directory with the -w flag.

```
kusion generate (-w DIRECTORY) [flags]
```

### Examples

```

		# Generate spec with working directory
		kusion generate -w /path/to/stack

		# Generate spec with custom workspace
		kusion generate -w /path/to/stack --workspace dev

		# Generate spec with custom backend
		kusion generate -w /path/to/stack --backend oss
```

### Options

```
      --backend string     The backend to use, supports 'local', 'oss' and 's3'.
  -h, --help               help for generate
  -w, --workdir string     The working directory for generate (default is current dir where executed).
      --workspace string   The name of target workspace to operate in.
```

### Options inherited from parent commands

```
      --profile string          Name of profile to capture. One of (none|cpu|heap|goroutine|threadcreate|block|mutex) (default "none")
      --profile-output string   Name of the file to write the profile to (default "profile.pprof")
```

### SEE ALSO

* [kusion](index.md)	 - Kusion is the Platform Orchestrator of KusionStack

###### Auto generated by spf13/cobra on 29-Mar-2024