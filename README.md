## A tool to find free time of multiple schedules

## Run
### Cargo
```sh
$ cargo run
```

## Data file
Data file must be in current working directory.
Data file name is `data.toml`, an example of data file is bellow:
```toml
meeting_length = 30

[[Persons]]
name = "Person one"
    [Persons.free_times]
        sat = [['08:00', '13:00']]
        sun = [['14:00', '22:00']]
        mon = [['08:00', '13:00']]
        tue = [['14:00', '22:00']]
        wed = [['08:00', '15:00']]
        thu = [['08:00', '22:00']]
        fri = [['08:00', '22:00']]

[[Persons]]
name = "Amin Sharifi"
    [Persons.free_times]
	    sat = [['16:00', '20:00']]
	    sun = [['08:00', '12:00']]
	    mon = [['16:00', '20:00']]
	    tue = [['08:00', '12:00']]
	    wed = [['16:00', '20:00']]
	    thu = [['08:00', '12:00'], ['14:00', '22:00']]
	    fri = [['08:00', '12:00'], ['14:00', '22:00']]

[[Persons]]
name = "Person two"
    [Persons.free_times]
	sat = [['11:00', '22:00']]
	sun = [['14:00', '22:00']]
	mon = [['11:00', '22:00']]
	tue = [['14:00', '22:00']]
	wed = [['11:00', '22:00']]
	thu = [['11:00', '22:00']]
	fri = [['08:00', '22:00']]

```

## License
Apache v2 or MIT by your choice
