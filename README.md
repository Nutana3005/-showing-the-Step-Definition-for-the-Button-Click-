# -showing-the-Step-Definition-for-the-Button-Click-
from behave import when

@when('I click the "{button_text}" button')
def step_impl(context, button_text):
    button = context.browser.find_element_by_text(button_text)
    button.click()
