# enable new Features
use Rex -feature => 1.3;

use Rex::Helper::SSH2;
use Rex::Commands;
use Data::Dumper;
use common::sense;
use Rex::Transaction;

user "rex";
private_key "/var/lib/jenkins/.ssh/id_rsa";
public_key "/var/lib/jenkins/.ssh/id_rsa.pub";
port "7022";

set group => "server" => "localhost";

task "uptime", group => "server", sub {
  say run "uptime";
  print $?;
};

1;
