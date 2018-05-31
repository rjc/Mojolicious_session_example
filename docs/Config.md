# Config

Let's talk about config files and the Config plugin.
Is there a better way than YAML files?

I really don't understand this right now.  I've got a $config in the 
router SessionTutorial.pm and a different one in the controller Tutorial.pm
They are separate entities (controller $config needs a my)

##  Mojolicious::Plugin::Config - Perl-ish configuration plugin

set the `MOJO_CONFIG` environment variable

`session_tutorial.conf` is not always read by default
make sure you load it with `use Mojolicious::Plugin::Config;`
and `$self->plugin('Config');`

And this bit by Luc Didry is interesting
```
my $config_file = catfile(qw(etc), $self->app->moniker.'.conf');
    my $config;
    if (-e $config_file) {
        $config = $self->plugin('Config', {file => $config_file});
    } 
```

## lib/SessionTutorial/Controller/Tutorial.pm

## lib/SessionTutorial.pm

# Try it out
With the server running,
click through the Login link on [localhost:3000/](http://localhost:3000/)
to get to the [Login page](http://localhost:3000/login)

#### TODO ####

# Test the app

```
script/session_tutorial test t/01_login.t
```

# Next Step

**This tutorial finishes here.**

Instructions continue in [Config](Config.md).

## More information
