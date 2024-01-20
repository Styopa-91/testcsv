Клики без екшенов:
select * from click 
left join actions on click.id = actions.click_id
where actions.click_id is null;

Клики с екшенами:
select * from click 
left join actions on click.id = actions.click_id
where actions.click_id is not null;
