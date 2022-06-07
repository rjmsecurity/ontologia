> 1.8 Given a scenario, configure Microsoft Windows networking on a client/desktop.

# Firewall advanced settings

- continuing off of [Firewall](../1.6%20Control%20Panel/Firewall.md) with the *Advanced settings* link in the left sidebar
- you can block or allow traffic to an app or feature based on a port number
- can also create exceptions to these restrictions
- combine these criteria together to create a custom rule in the custom rules section
- the left sidebar of the Advanced settings page has inbound rules, outbound rules, connection security rules, and monitoring
- e.g. inbound shows *all* of the inbound rules in your Firewall with a name column, group, public/private, enabled/disabled, allow/block/allow if secure, and more
- on the right sidebar, create a new rule > custom rule 
- from there select *apply to all programs* > block TCP (web server traffic), specifically port 80 > source and dest IP addresses 
- from there the actions are allow, block, or allow if the connection is secure
- apply for the domain, public, or private profiles?
- finally the wizard concludes by asking for a name for your rule