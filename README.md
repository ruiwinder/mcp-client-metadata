# mcp-client-metadata

`client.json` is an OAuth Client ID Metadata Document. Its URL,
`https://ruiwinder.github.io/mcp-client-metadata/client.json`, is the OAuth
client ID a local MCP client (magpie) uses to sign in to MCP servers that
accept metadata documents instead of dynamic client registration, with PKCE
and no client secret.

Keep the file at this URL: the `client_id` field has to equal the URL, and
the authorization server reads it again on later sign-ins. Do not add
redirect URIs other than the loopback ones.
