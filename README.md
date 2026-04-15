# gha-repository_dispatch-example
# run this from gitbash or vscode

                   curl -X POST \
                    -H "Accept: application/vnd.github+json" \
                    -H "Authorization: Bearer $GITHUB_TOKEN" \
                    https://api.github.com/repos/bestdevopsengineer/gha-repository_dispatch-example/dispatches \
                    -d '{"event_type": "trigger-deploy", "client_payload": {"message": "hello from outside"}}'

