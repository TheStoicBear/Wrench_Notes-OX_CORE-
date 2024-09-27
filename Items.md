['note'] = {
    label = 'Note',
    weight = 10,
    stack = true,
    close = true,
    client = {
        anim = { dict = 'amb@world_human_clipboard@male@idle_a', clip = 'idle_c' }, -- Optional animation when opening note
        prop = {
            model = 'prop_notepad_01', -- Optional model for note
            pos = { x = 0.03, y = 0.03, z = -0.02},
            rot = { x = 0.0, y = 0.0, z = 0.0}
        },
        usetime = 1000, -- Optional delay for opening the note
        use = function()
            -- Open the note UI when the item is used
            exports['your_resource_name']:OpenNoteUI()
        end
    }
}
