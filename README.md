This is a demonstration inspired by [SysmteKit](https://github.com/beltex/SystemKit).

The official [SystemKit](https://github.com/beltex/SystemKit) example require XCode editor to build and run since the
repository was packaged as a module. This project is meant to use command line to compile and run the example file with
source file of SystemKit as libraries.

## How to compile

```
$ swiftc -o output main.swift System.swift
```

Note: If you are new to command line Swift, `swift` command is a interperter to run Swift code or enter Swift
interactive mode. To compile Swift file, you should use `swiftc` instead. (It's similar to `java` and `javac`)

Alternatively, you can compile the source files with:

```
$ xcrun -sdk macosx swiftc -emit-executable -o output main.swift System.swift
```

## How to run 

```
$ ./output
// MACHINE STATUS

-- CPU --
	PHYSICAL CORES:  2
	LOGICAL CORES:   4
	SYSTEM:          8%
	USER:            12%
	IDLE:            79%
	NICE:            0%

-- MEMORY --
	PHYSICAL SIZE:   16.0GB
	FREE:            223MB
	WIRED:           3.60GB
	ACTIVE:          5.00GB
	INACTIVE:        4.90GB
	COMPRESSED:      2.27GB

-- SYSTEM --
	MODEL:           MacBookPro14,1
	UPTIME:          26d 4h 56m 52s
	PROCESSES:       647
	THREADS:         3474
	LOAD AVERAGE:    ["2.48", "2.32", "2.53"]
	MACH FACTOR:     [2.024, 1.992, 1.99]

-- POWER --
	CPU SPEED LIMIT: 100.0%
	CPUs AVAILABLE:  4
	SCHEDULER LIMIT: 100.0%
	THERMAL LEVEL:   Not Published
```
