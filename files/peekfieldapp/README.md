SSH to the peek server, and run the following

```````[ "${USER}" == 'peek' ] || echo "You are NOT the peek user" >&2
cd

tar cvjf $(date "+%y%m%d_%H%M")_peek_field_app.tar.bz2 \
    --exclude node_modules \
    -C synerty-peek*/lib/python*/site-packages \
    peek_field_app

