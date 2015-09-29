
# NAME

Mojolicious::Plugin::ClientIP - Get client's IP address from X-Forwarded-For

# SYNOPSIS

    use Mojolicious::Lite;

    plugin 'ClientIP';

    get '/' => sub {
        my $c = shift;
        $c->render(text => $c->client_ip);
    };

    app->start;

# DESCRIPTION

Mojolicious::Plugin::ClientIP is a Mojolicious plugin to get an IP address looks like client, not proxy, from X-Forwarded-For header.

# LICENSE

Copyright (C) Six Apart, Ltd. <sixapart@cpan.org>

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# AUTHOR

ziguzagu <ziguzagu@cpan.org>
