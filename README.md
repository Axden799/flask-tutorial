# flask-tutorial
Tutorial app made with Flask.

To run flask in local development server,  use:

flask --app flaskr run --debug 

pytest results:

============================================================================= test session starts ==============================================================================
platform darwin -- Python 3.12.2, pytest-8.1.1, pluggy-1.4.0 -- /Users/denisdutka/Public/repos/flask-tutorial/venv/bin/python3.12
cachedir: .pytest_cache
rootdir: /Users/denisdutka/Public/repos/flask-tutorial
configfile: pyproject.toml
collected 24 items                                                                                                                                                             

test_auth.py::test_register PASSED                                                                                                                                       [  4%]
test_auth.py::test_register_validate_input[--Username is required.] PASSED                                                                                               [  8%]
test_auth.py::test_register_validate_input[a--Password is required.] PASSED                                                                                              [ 12%]
test_auth.py::test_register_validate_input[test-test-already registered] PASSED                                                                                          [ 16%]
test_auth.py::test_login PASSED                                                                                                                                          [ 20%]
test_auth.py::test_login_validate_input[a-test-Incorrect username.] PASSED                                                                                               [ 25%]
test_auth.py::test_login_validate_input[test-a-Incorrect password.] PASSED                                                                                               [ 29%]
test_auth.py::test_logout PASSED                                                                                                                                         [ 33%]
test_blog.py::test_index PASSED                                                                                                                                          [ 37%]
test_blog.py::test_login_required[/create] PASSED                                                                                                                        [ 41%]
test_blog.py::test_login_required[/1/update] PASSED                                                                                                                      [ 45%]
test_blog.py::test_login_required[/1/delete] PASSED                                                                                                                      [ 50%]
test_blog.py::test_author_required PASSED                                                                                                                                [ 54%]
test_blog.py::test_exists_required[/2/update] PASSED                                                                                                                     [ 58%]
test_blog.py::test_exists_required[/2/delete] PASSED                                                                                                                     [ 62%]
test_blog.py::test_create PASSED                                                                                                                                         [ 66%]
test_blog.py::test_update PASSED                                                                                                                                         [ 70%]
test_blog.py::test_create_update_validate[/create] PASSED                                                                                                                [ 75%]
test_blog.py::test_create_update_validate[/1/update] PASSED                                                                                                              [ 79%]
test_blog.py::test_delete PASSED                                                                                                                                         [ 83%]
test_db.py::test_get_close_db PASSED                                                                                                                                     [ 87%]
test_db.py::test_init_db_command PASSED                                                                                                                                  [ 91%]
test_factory.py::test_config PASSED                                                                                                                                      [ 95%]
test_factory.py::test_hello PASSED                                                                                                                                       [100%]


Code Coverage:

Name                                                               Stmts   Miss  Cover
--------------------------------------------------------------------------------------
/Users/denisdutka/Public/repos/flask-tutorial/flaskr/__init__.py      27      1    96%
/Users/denisdutka/Public/repos/flask-tutorial/flaskr/auth.py          60      0   100%
/Users/denisdutka/Public/repos/flask-tutorial/flaskr/blog.py          60      0   100%
/Users/denisdutka/Public/repos/flask-tutorial/flaskr/db.py            23      0   100%
conftest.py                                                           33      0   100%
test_auth.py                                                          30      0   100%
test_blog.py                                                          59      0   100%
test_db.py                                                            19      0   100%
test_factory.py                                                        7      0   100%
--------------------------------------------------------------------------------------
TOTAL                                                                318      1    99%
