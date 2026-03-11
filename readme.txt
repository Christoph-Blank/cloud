https://supabase.com/dashboard/sign-in


mama@proton.me
papa@proton.me
oliver@proton.me
isabell@proton.me

admin@proton.me


bei SQL mit folgenden befehlen die recht an den Ordner vergeben:

Admin
  update auth.users
  set raw_user_meta_data = '{"role":"admin","email_verified":true}'
  where email = 'admin@proton.me';

Benutzer
  update auth.users
  set raw_user_meta_data = '{"folder":"Isabell"}'
  where email = 'isabell@proton.me';

  update auth.users
  set raw_user_meta_data = '{"folder":"Oliver"}'
  where email = 'oliver@proton.me';

  update auth.users
  set raw_user_meta_data = '{"folder":"Papa"}'
  where email = 'papa@proton.me';

  update auth.users
  set raw_user_meta_data = '{"folder":"Mama"}'
  where email = 'mama@proton.me';
